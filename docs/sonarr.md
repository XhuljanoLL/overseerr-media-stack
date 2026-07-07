# Sonarr

Before starting the stack, copy [.env.example](../.env.example) to .env and adjust the values for your machine, especially the host paths used by the bind mounts.

Sonarr manages TV show libraries and works with Prowlarr and qBittorrent in this stack.

## First-time setup

- Open the web UI at <http://localhost:8989>.
- Add your TV show library root folder and point it to the mounted TV show path used by the container.
- Connect Sonarr to Prowlarr for indexers and to qBittorrent for downloads.
- Create quality profiles and set your preferred release profile behavior.
- Double-check that the download and library paths match the volumes configured in the compose file.

## Helpful links

- Official wiki: <https://wiki.servarr.com/sonarr>
- Related stack guides: [Prowlarr](./prowlarr.md), [qBittorrent](./qbitorrent.md)

## What to configure

- Open the web UI at <http://localhost:8989>.
- Add your TV show library root folder and point it to the mounted TV show path used by the container.
- Connect Sonarr to Prowlarr for indexers and to qBittorrent for downloads.
- Create quality profiles and set your preferred release profile behavior.

## Notes for this setup

- The compose file mounts the TV library to /data/tvshows inside the container.
- The download folder is exposed to the container at /data/downloads.
- If you change the host paths, make sure the same paths are reflected in Sonarr settings.
