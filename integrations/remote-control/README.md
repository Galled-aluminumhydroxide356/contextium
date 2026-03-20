# Remote Control

Mobile access to your AI agent for text-based interaction from phone or tablet.

## Requirements

- Host machine running the agent service
- Mobile client app or web interface

## Setup

1. Deploy the remote control service on your host machine
2. Configure as a systemd service for persistence
3. Set up secure access (VPN, tunnel, or Zero Trust)
4. Install the mobile client or bookmark the web interface

## Architecture

```
Mobile Device → Secure Tunnel → Host Machine → AI Agent
```

## Use Cases

- Sending quick queries to your AI from your phone
- Checking on automation status while away from desk
- Creating tasks or journal entries on the go
- Getting quick answers from your knowledge base
