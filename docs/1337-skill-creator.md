# 1337-skill-creator

Create opinionated, best-in-class skills. Composes with `example-skills:skill-creator`.

## The 1337 Difference

| Standard Skill | 1337 Skill |
|----------------|------------|
| "Options include A, B, C" | "Use A. B is deprecated, C doesn't scale." |
| Explains how things work | Decision frameworks for what to pick |
| Comprehensive coverage | Production gotchas only |
| Tutorial-style | Tables and trees |

## How to Use

1. Load `example-skills:skill-creator` first (Anthropic's canonical guide)
2. Load `1337-skill-creator` (adds opinionated layer)
3. Follow the methodology

## Core Principles

1. **Best-in-class only** - THE answer, not catalogs
2. **Evidence over opinion** - Production usage > GitHub stars
3. **Concise** - Decision frameworks + gotchas, not tutorials
4. **Claude is smart** - Only add what Claude doesn't already know

## Content Triage

Quick test for every piece of content:

```
Does Claude know this? → YES → Is there an elite twist? → NO → CUT
```

## Reference Files

```
references/
├── content-triage.md   # Full content filtering methodology
└── skill-process.md    # End-to-end creation workflow
```

## Triggers

This skill activates when you're:
- Building new skills
- Designing skill structure
- Writing SKILL.md files
- Triaging research content
- Creating opinionated documentation
