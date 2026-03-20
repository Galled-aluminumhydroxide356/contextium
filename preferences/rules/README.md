# Rules Index

Behavioral and governance rules with enforcement status.

## Rule Files

| File | Scope |
|------|-------|
| [behavior.md](behavior.md) | Delegation, context efficiency, depth policy, proactive value |
| [governance.md](governance.md) | Credentials, repo hygiene, project lifecycle, session end, people |

## Enforcement

| Rule | Source | Enforced by |
|------|--------|-------------|
| Delegation-first | `behavior.md` | Manual |
| Context efficiency | `behavior.md` | Hook (optional) |
| Depth policy | `behavior.md` | Manual |
| Proactive value | `behavior.md` | Manual |
| Credential handling | `governance.md` | Manual |
| Repo hygiene | `governance.md` | Manual |
| Project lifecycle | `governance.md` | Manual |
| Session end / journal | `governance.md` | Manual |
| People & entities | `governance.md` | Manual |

## Hooks (Optional)

Hooks can be configured in your AI agent's settings to enforce rules automatically. Examples:
- Block writes to sensitive directories
- Remind to load integration docs before API calls
- Track file reads and suggest delegation
- Session start checklist
