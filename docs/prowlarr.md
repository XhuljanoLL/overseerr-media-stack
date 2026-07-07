# Prowlarr

Before starting the stack, copy [.env.example](../.env.example) to .env and adjust the values for your machine, especially the host paths used by the bind mounts.

Prowlarr is the indexer manager used by the Arr stack in this repository. It is the place where you connect your indexers, define applications, and link the download client.

## First-time setup

- Open the web UI at <http://localhost:9696>.
- Add your preferred indexers and enable the ones you actually use.
- Connect Prowlarr to Sonarr and Radarr so they can use the same indexers.
- Point the download client to the same qBittorrent instance used by the stack.
- If this is your first run, verify the app URLs and API keys before you save the connections.

## Helpful links

- Official wiki: <https://wiki.servarr.com/prowlarr>
- Related stack guides: [Radarr](./radarr.md), [Sonarr](./sonarr.md), [qBittorrent](./qbitorrent.md)

## What to configure

- Open the web UI at <http://localhost:9696>.
- Add your preferred indexers and enable the ones you actually use.
- Connect Prowlarr to Sonarr and Radarr so they can use the same indexers.
- Point the download client to the same qBittorrent instance used by the stack.

## Notes for this setup

- The compose file mounts the config folder to P:\Prowlarr\Config on Windows.
- The backup and download paths are also mapped from the Windows host, so keep those paths consistent if you change them.
- If you change the qBittorrent container port or host port, update the client settings in Prowlarr as well.
