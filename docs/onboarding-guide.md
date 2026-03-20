# Onboarding Guide

This guide defines the quick onboarding experience. When a user says "let's onboard", the AI loads this file and walks them through setup.

## How This Works

The onboarding is a 5-minute interactive conversation — not a monologue. Ask questions, adapt to responses, skip what's irrelevant.

---

## Step 1: Welcome (30 seconds)

**Say:**
"Welcome to Contextium — your AI's persistent context system. This repo gives me memory across sessions. The more we use it, the smarter I get about your life and work. Let's set you up in about 5 minutes."

**Ask:** "What's your name?"

**Action:** Note it for file creation.

---

## Step 2: AI Agent (30 seconds)

**Ask:** "What AI tool are you using? Claude Code, Cursor, or Codex CLI?"

**Action:** Based on their answer, copy the appropriate config from `agent-configs/` to the repo root:
- Claude Code → copy `agent-configs/claude/CLAUDE.md` to `./CLAUDE.md`, copy `AGENTS.md` and `GEMINI.md`
- Cursor → copy `agent-configs/cursor/.cursorrules` to `./.cursorrules` (when available)
- Codex → copy `agent-configs/codex/AGENTS.md` to `./AGENTS.md` (when available)

---

## Step 3: Preferences (2 minutes)

**Ask these questions conversationally:**
1. "How do you prefer AI communication — concise and direct, or thorough with explanations?"
2. "What do you do professionally? Multiple roles are fine."
3. "What's your primary goal with AI? Productivity? Learning? Building systems?"

**Action:** Create `preferences/user/preferences.md` with their answers:
```yaml
# User Preferences

## Communication
- Style: [concise/thorough]
- Tone: [direct/diplomatic]

## Working Style
- Role: [their answer]
- Primary AI goal: [their answer]

## AI Assistant Notes
- [any specific preferences mentioned]
```

---

## Step 4: First Knowledge Domain (1 minute)

**Ask:** "What's one area of your life you'd like me to have persistent context about? Common choices: work, health, finance, relationships, hobbies, a specific project."

**Action:** Create the knowledge domain:
- `knowledge/{domain}/README.md` with a brief description
- `knowledge/people/{their-name}/README.md` with their basic info

---

## Step 5: Done (30 seconds)

**Say:**
"Your Contextium is set up. Here's what I now know:
- Your preferences (how to communicate with you)
- Your first knowledge domain ({domain})
- Your profile

Every session from here builds on the last. When you're done working, just say 'close this out' and I'll journal what we did and commit.

**Want to go deeper?** Check `projects/setup/` — there are pre-built guides for:
- Connecting integrations (Google, Todoist, etc.)
- Building people cards
- Setting up health tracking
- Creating your first automation
- Configuring a morning briefing

Pick any that interest you, or just start working — we'll build context as we go."

**Action:**
1. Mark the onboarding project as complete
2. Create first journal entry
3. Commit and push
