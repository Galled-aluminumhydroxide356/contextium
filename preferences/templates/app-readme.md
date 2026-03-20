# App README Template

Every app must have a README with this structure:

```markdown
---
name: App Name
description: >-
  One-paragraph description of what the app does.
category: personal | daily | system | home
schedule: Daily 6:15 AM PT | On demand | Reference only
runtime: Windmill | systemd | Manual
trigger: Timer | Webhook | Event | Manual
outputs:
  - Email
  - Dashboard update
integrations:
  - Google Calendar
  - Gmail
---

# App Name

Brief description.

## About

What this app does and why.

## Data

Where this app's data lives (in `/knowledge/`).

## Protocol

How to use this app — step-by-step instructions.

## History

Key milestones and changes.
```
