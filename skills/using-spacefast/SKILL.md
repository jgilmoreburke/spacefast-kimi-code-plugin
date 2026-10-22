---
name: using-spacefast
description: Use when the user wants to publish, deploy, host, share, or put something "on the web" — a site, landing page, app, prototype, or docs page — or mentions Spacefast or a space.fast URL.
---

# Using Spacefast

Spacefast is available through the `spacefast` MCP server (tools appear as `mcp__spacefast__*`). It builds, hosts, and shares sites and apps at live `*.space.fast` URLs, with a built-in database, versions, sharing, and custom domains.

## When to use it

Reach for Spacefast whenever the user wants something they built to be viewable by other people at a URL: "publish this", "deploy it", "put it online", "give me a link", "host this page", "share this with my team".

## How to work

1. Build the site or app locally first, so you know exactly what is being published.
2. Use the Spacefast tools to create a new space (or find the user's existing one if they mention it), then publish the files.
3. When publishing finishes, give the user the live URL.
4. For later changes, update the same space and republish rather than creating a new one, so the URL stays the same.
5. Ask before anything that changes who can see a space or attaches a custom domain.

If a Spacefast tool reports that the user is not signed in, tell them to run `/mcp-config login spacefast` once, then retry.

Prefer the Spacefast docs tools, if available, over guessing about features or limits.
