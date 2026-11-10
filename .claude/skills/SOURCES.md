# Skill sources

These skills were copied by hand from shallow clones on 2026-11-10 after their contents were reviewed. All of them are Markdown only, with no scripts. To update one, re-copy it from upstream and review the diff first.

| Skill | Upstream | Commit |
|---|---|---|
| frontend-design | github.com/anthropics/skills `skills/frontend-design` | 2c5958e |
| vercel-react-best-practices | github.com/vercel-labs/agent-skills `skills/react-best-practices` | 1a2c79d |
| web-design-guidelines | github.com/vercel-labs/agent-skills `skills/web-design-guidelines` | 1a2c79d |
| next-dev-loop | github.com/vercel/next.js `skills/next-dev-loop` | 0425855a |
| next-bundle-optimizer | github.com/vercel/next.js `skills/next-bundle-optimizer` | 0425855a |
| storefront-best-practices | github.com/medusajs/medusa-agent-skills `plugins/ecommerce-storefront/skills/storefront-best-practices` | 42b9afd |

Notes:
- `web-design-guidelines` fetches the latest rules from raw.githubusercontent.com/vercel-labs/web-interface-guidelines each time it runs.
- `next-dev-loop` can use the `agent-browser` CLI, which isn't installed here. Use the built-in browser or Playwright in its place, or install the CLI on purpose.
