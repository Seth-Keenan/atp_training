@AGENTS.md

## Project

Ecommerce storefront built on Next.js 16 (App Router, Turbopack), React 19 and Tailwind CSS v4 (CSS-first config in `app/globals.css`, no `tailwind.config`). The backend, payments and component library haven't been chosen yet.

## Agent tooling in this workspace

Skills (`.claude/skills/`, copied from upstream; sources and commits in `.claude/skills/SOURCES.md`):

- `storefront-best-practices`: patterns for product pages, PLP, cart, checkout, navigation, SEO and mobile. Use it for any storefront page or component.
- `frontend-design`: sets the visual direction (type, color, layout) so the UI doesn't look like a template.
- `web-design-guidelines`: audits UI code for accessibility, UX and interaction quality.
- `vercel-react-best-practices`: React and Next.js performance rules (data fetching, bundles, re-renders).
- `next-dev-loop`: checks changes against the running dev server via `/_next/mcp`.
- `next-bundle-optimizer`: audits client bundle size and initial-load cost.

MCP servers (`.mcp.json`):

- `next-devtools`: reads routes, errors, logs and compile issues from the running `npm run dev`.
- `shadcn`: browses shadcn/ui registries and adds components from them. Run `npx shadcn@latest init` first to create `components.json`.
- `stripe`: the Stripe API and docs, after OAuth through `/mcp`. Use test mode only.

## Workflow

- Before writing Next.js code, read the matching guide in `node_modules/next/dist/docs/` (see AGENTS.md).
- After an edit, check the page in the running dev server (`next-dev-loop`, or the built-in browser), not only with types or lint.
- Store style tokens (colors, radii, fonts) under `@theme` in `app/globals.css`. Don't hard-code hex values in components.
