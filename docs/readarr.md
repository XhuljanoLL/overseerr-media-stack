# Readarr

Readarr is an optional book-management service for this stack. It is not active in the main compose file, but it can be enabled from the additional services configuration if you want to manage ebooks and audiobooks.

## First-time setup

- If you enable it, open the web UI at <http://localhost:8787>.
- Point Readarr to your books library and download path.
- Connect it to Prowlarr and your download client for automation.
- Create a quality profile that matches the content you want to track.

## Helpful links

- Official wiki: <https://wiki.servarr.com/readarr>
- Related stack guide: [Prowlarr](./prowlarr.md), [qBittorrent](./qbitorrent.md)

## What to configure

- Open the web UI at <http://localhost:8787> if you enable it.
- Point Readarr to your books library and download path.
- Connect it to Prowlarr and your download client for automation.

## Notes for this setup

- The service expects a host path for /config and a books storage path.
- If you use it, update the Windows bind mounts to match your local layout.
- It is optional and does not affect the active base stack unless enabled.
