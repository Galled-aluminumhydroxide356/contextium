---
project: setup-integrations
status: pending
created: auto
tags: [setup]
---

# Setup: Connect Your Integrations

## Goal

Connect the external services you use to your Contextium repo.

## Steps

- [ ] **Credential Vault** — Set up 1Password (or your preferred vault) for API key storage
  - Install the CLI tool
  - Create a service account
  - Configure environment variables
- [ ] **Google Workspace** — Connect Google APIs (Calendar, Gmail, Drive, etc.)
  - Create a Google Cloud project
  - Set up OAuth2 credentials
  - Run the initial auth flow
- [ ] **Task Manager** — Connect Todoist (or your preferred task tool)
  - Generate an API key
  - Test with a simple task creation
- [ ] **Automation Platform** — Set up Windmill or n8n
  - Deploy or sign up for an instance
  - Configure API access
  - Deploy your first workflow
- [ ] **Other Services** — Browse `integrations/` for connectors relevant to your stack

## Notes

- Configure only what you need — you can always add more later
- Each integration's README has detailed setup steps
- Store all credentials in your vault, never on disk
