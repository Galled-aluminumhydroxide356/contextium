# Google Workspace

Access Google APIs including Drive, Sheets, Gmail, Calendar, and Contacts.

## Requirements

- Google Cloud project with relevant APIs enabled
- OAuth2 credentials (client ID + client secret)
- Authorized redirect URI configured

## Setup

1. Create a Google Cloud project at console.cloud.google.com
2. Enable APIs: Gmail, Calendar, Drive, Sheets, Contacts
3. Create OAuth2 credentials (Desktop or Web app type)
4. Store client ID and secret in your credential vault
5. Run the auth flow via `integrations/google-auth/`

## Key APIs

| API | Scope | Use |
|-----|-------|-----|
| Gmail | `gmail.send`, `gmail.readonly` | Send and read emails |
| Calendar | `calendar.readonly`, `calendar.events` | Read/write events |
| Drive | `drive.readonly`, `drive.file` | File access |
| Sheets | `spreadsheets` | Read/write spreadsheets |
| Contacts | `contacts.readonly` | Contact lookup |

## Token Management

- Tokens auto-refresh when expired
- If refresh token is revoked, re-run the auth flow
- Supports multiple accounts (personal, work)

## Use Cases

- Sending daily briefing emails via Gmail
- Reading calendar events for agenda planning
- Writing data to Google Sheets for tracking
- Looking up contact information
