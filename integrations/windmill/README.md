# Windmill

Self-hosted workflow automation platform for scheduled jobs, webhooks, and multi-step workflows.

## Requirements

- Windmill instance (self-hosted or cloud)
- API token with workspace access

## Setup

1. Deploy Windmill or use the cloud instance
2. Create a workspace
3. Generate an API token: Settings > Tokens
4. Store the instance URL and token in your credential vault
5. Install the CLI: `npm install -g windmill-cli`

## Key Operations

```bash
wmill sync pull          # Pull workspace scripts locally
wmill sync push          # Push local changes to Windmill
wmill flow run <path>    # Trigger a flow manually
```

## Deployment Workflow

1. Edit scripts locally in your repo
2. Test locally if possible
3. Push to Windmill via CLI: `wmill sync push`
4. Verify in the Windmill UI

## Use Cases

- Scheduled data syncs (cron-triggered)
- Webhook handlers for external services
- Multi-step workflows (fetch, transform, deliver)
- Background jobs that run without user interaction
