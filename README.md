# content-audit-skill

> Built by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **The GEO Lab** · [𝕏 @TheGEO\_Lab](https://x.com/TheGEO_Lab) · [LinkedIn](https://linkedin.com/in/arturgeo) · [Reddit](https://www.reddit.com/user/Alternative_Teach_74/)

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Licence](https://img.shields.io/badge/licence-MIT-green)
![Claude Code](https://img.shields.io/badge/Claude_Code-skill-blueviolet)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/arturseo-geo/content-audit-skill/blob/main/CONTRIBUTING.md)

Post-publication content maintenance skill for [Claude Code](https://docs.anthropic.com/en/docs/claude-code). Audit published content for GEO compliance, detect freshness decay, test LLM readability at the section level, and manage citation rate re-test schedules.

## Why This Exists

Content quality degrades after publication. Statistics become outdated. Competitors publish better-structured answers. Citation rates decay silently. Traditional SEO tools don't catch these GEO-specific failures because they don't measure passage-level retrievability.

This skill fills the maintenance gap in the content lifecycle:

**seo-geo** (plan) → **content-pipeline** (create) → **content-audit** (maintain)

## What It Does

| Capability | Reference File | What it checks |
|-----------|---------------|----------------|
| **GEO Compliance Audit** | `references/compliance-checklist.md` | 25 checks: schema, structure, voice, links, CTAs |
| **Section Quality Gate** | `references/geo-quality-gate.md` | 5 per-section questions: direct opener, pronouns, single topic, data, citation-readiness |
| **Content Freshness** | `references/content-freshness.md` | Statistical currency, 4-priority framework, 7-step update protocol |
| **LLM Readability** | `references/llm-readability.md` | 7-component passage-level test mapped to GEO Stack layers |
| **Re-Test Cadence** | `references/retest-cadence.md` | 5 mandatory triggers, 6-month baseline, citation rate tracking log |

## Install

```bash
# Clone
git clone https://github.com/arturseo-geo/content-audit-skill.git ~/.claude/skills/content-audit

# Or install all skills at once
git clone https://github.com/arturseo-geo/claude-code-skills.git
cp -r claude-code-skills/skills/content-audit ~/.claude/skills/
```

## File Structure

```
content-audit-skill/
├── SKILL.md                           — Core skill instructions and audit workflow
└── references/
    ├── compliance-checklist.md         — 25-check GEO compliance audit
    ├── geo-quality-gate.md             — 5-question per-section quality gate
    ├── content-freshness.md            — Freshness decay detection and update protocol
    ├── llm-readability.md              — 7-component LLM readability test
    └── retest-cadence.md               — Citation rate re-test scheduling
```

## Usage

Once installed, Claude Code auto-triggers this skill when you mention content auditing, compliance, freshness, or maintenance:

```
> audit this page for GEO compliance
> check if the statistics on /retrieval-probability/ are still current
> test the LLM readability of this H2 section
> when should I re-test citation rates on our core pages?
> is this opening sentence citation-ready?
```

## The Content Lifecycle

| Stage | Skill | What it does |
|-------|-------|--------------|
| **Plan** | [seo-geo-skill](https://github.com/arturseo-geo/seo-geo-skill) | Keyword research, SERP analysis, content strategy |
| **Create** | [content-pipeline-skill](https://github.com/arturseo-geo/content-pipeline-skill) | 7-agent pipeline: research, write, edit, optimise, review |
| **Maintain** | **content-audit-skill** (this repo) | Compliance audit, freshness, readability, re-test cadence |

## Related Repos

- [claude-code-skills](https://github.com/arturseo-geo/claude-code-skills) — All 18 skills in one collection
- [seo-geo-skill](https://github.com/arturseo-geo/seo-geo-skill) — SEO & GEO optimisation (plan stage)
- [content-pipeline-skill](https://github.com/arturseo-geo/content-pipeline-skill) — Multi-agent content production (create stage)
- [grounded-research-skill](https://github.com/arturseo-geo/grounded-research-skill) — Anti-hallucination research mode

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. PRs welcome.

---

Built and maintained by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **[The GEO Lab](https://thegeolab.net)** · [MIT License](LICENSE)
