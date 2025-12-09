# Contributing

Elite skills for Claude Code. Best-in-class only.

## Before You Start

1. Read **CLAUDE.md** - architecture, conventions, skill authoring rules
2. Load **1337-skill-creator** skill - methodology for creating skills
3. Check if there's an existing skill that should be updated instead

## Adding a Skill

```
plugins/your-skill/
├── SKILL.md           # Required: decisions + gotchas (100-200 lines)
└── references/        # Optional: domain-specific deep dives
```

Update `marketplace.json`:
```json
{
  "name": "your-skill",
  "source": "./plugins/your-skill",
  "description": "What + Use when: triggers (max 600 chars)",
  "version": "0.1.0",
  "skills": ["./"]
}
```

## Quality Standards

| Do | Don't |
|----|-------|
| Pick THE answer | List catalogs of options |
| Cite evidence (production usage) | State opinions |
| Decision frameworks + gotchas | Complete tutorials |
| Tables and trees | Verbose prose |

## Checklist

- [ ] Description < 600 chars with "Use when:" triggers
- [ ] SKILL.md is decisions, not tutorial (100-200 lines)
- [ ] Each recommendation has evidence
- [ ] No catalogs - clear winners picked
- [ ] References linked, not embedded

## Commit Format

```
Add/Update [skill]: [brief description]

[Evidence or reasoning]

🤖 Generated with [Claude Code](https://claude.com/claude-code)

Co-Authored-By: Claude <noreply@anthropic.com>
```

## Auto-Updates

Skills auto-update monthly via GitHub Action. For manual updates:
1. Run `/skill-update` command
2. Research current state
3. Update only with evidence
4. Create PR for review

## License

MIT. By contributing, you agree your contributions will be licensed under MIT.
