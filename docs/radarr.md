# Radarr

Before starting the stack, copy [.env.example](../.env.example) to .env and adjust the values for your machine, especially the host paths used by the bind mounts.

Radarr manages movie libraries and works with Prowlarr and qBittorrent in this stack.

## First-time setup

- Open the web UI at <http://localhost:7878>.
- Add your movie library root folder and point it to the mounted movie path used by the container.
- Connect Radarr to Prowlarr for indexers and to qBittorrent for downloads.
- Create at least one quality profile and one profile for your preferred movie quality.
- Verify the download folder and movie root folder paths match the ones configured in the compose file.

## Helpful links

- Official wiki: <https://wiki.servarr.com/radarr>
- Related stack guides: [Prowlarr](./prowlarr.md), [qBittorrent](./qbitorrent.md)

## What to configure

- Open the web UI at <http://localhost:7878>.
- Add your movie library root folder and point it to the mounted movie path used by the container.
- Connect Radarr to Prowlarr for indexers and to qBittorrent for downloads.
- Create at least one quality profile and one profile for your preferred movie quality.

## Notes for this setup

- The compose file mounts the movie library to /data/movies inside the container.
- The download folder is exposed to the container at /data/downloads.
- If you change the host paths, make sure the same paths are reflected in Radarr settings.
