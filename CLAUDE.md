# Contextium

> Give your AI an operating system.

This is a Contextium repo — a structured context system that gives your AI assistant persistent memory across sessions.

## Getting Started

If this is your first time, say **"let's onboard"** and I'll walk you through a 5-minute setup.

If you've already onboarded, I'll use the context router below to load what's relevant.

## Context Router

| Trigger | Load |
|---------|------|
| Every session | `preferences/user/preferences.md` |
| Non-trivial task | `knowledge/growth/goals/current-focus.md` |
| Project work | `projects/README.md` |
| Any integration/API call | `integrations/{name}/README.md` |
| Person mentioned | `knowledge/people/{name}/` |
| Prior work referenced | `journal/` (latest) |

## Repo Structure

| Directory | Purpose |
|-----------|---------|
| `apps/` | App protocols + automation scripts |
| `knowledge/` | Domain-organized reference data |
| `projects/` | Time-boxed work items |
| `journal/` | Daily session logs |
| `preferences/` | User preferences, rules, templates |
| `integrations/` | External service connectors |
| `agent-configs/` | AI agent instruction files |

## Rules

See `preferences/rules/` for behavioral and governance rules.

## Onboarding

When the user says "let's onboard", "onboard me", or "start onboarding":
1. Load `docs/onboarding-guide.md`
2. Begin the guided setup (5 questions, ~5 minutes)
3. Copy the appropriate agent config based on their AI tool choice
