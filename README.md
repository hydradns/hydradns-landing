# HydraDNS Landing

The marketing and docs site for [HydraDNS](https://github.com/hydradns/hydradns), a self-hosted DNS-layer security and privacy gateway. This is a standalone Vite + React + TypeScript + Tailwind app, kept in its own repo separate from the product monorepo.

Live at [hydradns.app](https://hydradns.app).

## Running locally

```sh
npm ci
npm run dev
```

Opens on `http://localhost:8080` by default (or `:3001` in the full stack's Docker Compose setup).

## Build

```sh
npm run build
```

Outputs a static bundle to `dist/`, served in production behind Nginx (see `Dockerfile`).

## Test

```sh
npm run test        # vitest, single run
npm run test:watch  # vitest, watch mode
```

## Lint

```sh
npm run lint
```

## Where things live

- `src/components/` — landing page sections (Hero, Features, Comparison, etc.)
- `src/pages/docs/` — the `/docs` route: written documentation pages, rendered as React components, not a separate subdomain
- `public/` — static assets, icons, and the social-preview image

## The main project

The DNS engine, dashboard, CLI, and scanner live in the [hydradns/hydradns](https://github.com/hydradns/hydradns) monorepo. This repo only contains the marketing site and its docs content.
