# Overseerr

Overseerr is an optional request-management frontend for your media stack. It is not part of the currently active main compose file, but it can be enabled later if you want a simple interface for media requests.

## First-time setup

- If you enable it, open the web UI at <http://localhost:5055>.
- Create your first admin account and sign in.
- Connect Overseerr to your Arr apps so requests can flow into Sonarr and Radarr.
- If you plan to use it remotely, configure your reverse proxy or local network access before exposing it.

## Helpful links

- Official documentation: <https://docs.overseerr.dev/>
- Related stack guide: [Radarr](./radarr.md), [Sonarr](./sonarr.md)

## What to configure

- Open the web UI at <http://localhost:5055> if you enable it.
- Connect it to your Arr apps so requests can flow into Sonarr and Radarr.
- Use your own reverse-proxy or local networking setup if you want external access.

## Notes for this setup

- The service was previously kept as an optional addition in the additional services file.
- If you re-enable it, make sure the host path for /config is updated to a real Windows folder.
- The service may need DNS adjustments in some environments, especially when using scraper-based tools.
