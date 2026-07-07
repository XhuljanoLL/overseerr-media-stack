# Lidarr

Lidarr is an optional music-management service for this stack. It is not active in the main compose file, but it can be enabled from the additional services configuration if you want to manage music libraries.

## First-time setup

- If you enable it, open the web UI at <http://localhost:8686>.
- Point Lidarr to your music library and download path.
- Connect it to Prowlarr and your download client so new releases can be fetched automatically.
- Create at least one quality profile that matches the albums you want to track.

## Helpful links

- Official wiki: <https://wiki.servarr.com/lidarr>
- Related stack guide: [Prowlarr](./prowlarr.md), [qBittorrent](./qbitorrent.md)

## What to configure

- Open the web UI at <http://localhost:8686> if you enable it.
- Point Lidarr to your music library and download path.
- Connect it to Prowlarr and your download client for automation.

## Notes for this setup

- The service expects a host path for /config and a music storage path.
- If you use it, update the Windows bind mounts to match your local layout.
- It is optional and does not affect the active base stack unless enabled.
