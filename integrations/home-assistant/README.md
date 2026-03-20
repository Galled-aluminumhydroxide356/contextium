# Home Assistant

Home automation API for device control and sensor data.

## Requirements

- Home Assistant instance (local or cloud)
- Long-lived access token

## Setup

1. Go to your HA instance: Profile > Security > Long-Lived Access Tokens
2. Create a token and store it in your credential vault
3. Store the instance URL (e.g., `http://homeassistant.local:8123`)
4. Test: `curl -H "Authorization: Bearer $TOKEN" http://ha-host:8123/api/`

## Key Endpoints

| Action | Method | Endpoint |
|--------|--------|----------|
| Get states | GET | `/api/states` |
| Get entity | GET | `/api/states/{entity_id}` |
| Call service | POST | `/api/services/{domain}/{service}` |
| Fire event | POST | `/api/events/{event_type}` |

## Common Services

```bash
# Turn on a light
POST /api/services/light/turn_on {"entity_id": "light.living_room"}

# Set thermostat
POST /api/services/climate/set_temperature {"entity_id": "climate.main", "temperature": 72}
```

## Use Cases

- Controlling lights, locks, and climate
- Reading sensor data (temperature, humidity, motion)
- Triggering automations from external events
- Building smart home dashboards
