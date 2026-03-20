# Changelog

All notable changes to Contextium are documented here.

## [1.0.0] — 2026-03-19

### Initial Release

**Core Framework:**
- Structured repo architecture with 6 layers (instruction files, apps, knowledge, integrations, preferences, projects + journal)
- Context router with lazy loading — loads only what's relevant per session
- Behavioral rules (delegation-first, context efficiency, depth policy)
- Governance rules (credentials, repo hygiene, project lifecycle, session discipline)
- `.gitattributes` merge strategy protecting user data during updates

**Onboarding:**
- 5-minute quick onboarding flow ("let's onboard")
- Dynamic agent config selection (Claude Code, Cursor, Codex)
- 5 pre-loaded setup projects (integrations, people cards, health tracking, automation, daily briefing)

**Sample Apps (6):**
- Shared Utilities (Utility pattern)
- Goals (Reference pattern)
- Health Tracker (Data Sync pattern)
- News Digest (Timer + Email pattern)
- Error Remediation (System/Event pattern)
- Today's Agenda (Briefing pattern)

**Integration Connectors (27):**
- Credential management (1Password)
- Productivity (Google Workspace, Todoist)
- Automation (Windmill, n8n)
- Infrastructure (Cloudflare, TrueNAS, Garage, Daedalus)
- AI agents (Codex, Gemini, Browse)
- Business tools (Autotask, NinjaOne, QuickBooks, Monarch, Strety, Hudu, MSPBots)
- Smart home (Home Assistant)
- Interfaces (TRMNL, Remote Control, HAPI, VS Code)

**Templates:**
- Journal entry format
- Project README format
- App README format
- Email template guide

**Installer:**
- `install.sh` with init (fresh install) and update (pull upstream) modes
- Protected path merging for user data
