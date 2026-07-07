# qBittorrent

Before starting the stack, copy [.env.example](../.env.example) to .env and adjust the values for your machine, especially the host paths used by the bind mounts.

qBittorrent is the download client used by Sonarr, Radarr, and Prowlarr in this stack. It is exposed on <http://localhost:8088> and uses the mounted download directory from the host.

## First-time setup

- Open the web UI at <http://localhost:8088>.
- Change the default credentials as soon as possible.
- Set the default download location to the mounted download folder used by the container.
- Make sure the Arr apps are pointing to the same client and the same download path.
- If you use a different host path, update the compose volume mapping before starting the container.

## Helpful links

- Official wiki: <https://github.com/qbittorrent/qBittorrent/wiki>
- Related stack guides: [Prowlarr](./prowlarr.md), [Radarr](./radarr.md), [Sonarr](./sonarr.md)

## What to configure

- Open the web UI at <http://localhost:8088>.
- Change the default credentials as soon as possible.
- Set the default download location to the mounted download folder used by the container.
- Make sure the Arr apps are pointing to the same client and the same download path.

## Notes for this setup

- The compose file maps the host download folder to /downloads inside the container.
- The config directory is stored on the Windows host at P:\qbittorrent\config.
- If you use a different host path, update the compose volume mapping before starting the container.
