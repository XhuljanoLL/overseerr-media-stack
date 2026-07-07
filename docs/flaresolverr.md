# FlareSolverr

Before starting the stack, copy [.env.example](../.env.example) to .env and adjust the values for your machine, especially the host paths used by the bind mounts.

FlareSolverr is used to help indexers and scraping tools bypass Cloudflare protections. In this stack it is available as an optional helper service for Prowlarr and related automation tools.

## First-time setup

- Open the web UI at <http://localhost:8191> after the container is running.
- Leave the service running if you rely on scraping-based indexers or any provider that needs Cloudflare bypass.
- If you use it with other services, point them at <http://flaresolverr:8191> from inside the Docker network.
- No extra account setup is normally required for the basic stack.

## Helpful links

- Official documentation: <https://github.com/FlareSolverr/FlareSolverr>
- Related stack guide: [Prowlarr](./prowlarr.md)

## What to configure

- Open the service at <http://localhost:8191>.
- Leave it running if you rely on scraping-based indexers.
- If you use it with other services, point them to <http://flaresolverr:8191> from inside the Docker network.

## Notes for this setup

- The compose file exposes the service on port 8191.
- It does not require a persistent data volume for the basic setup.
- If you do not use scraping-heavy indexers, you can leave it disabled without affecting the rest of the stack.
