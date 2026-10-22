# Spacefast for Kimi Code

Publish to the web from Kimi Code. This plugin adds the Spacefast MCP server, a `using-spacefast` skill loaded at session start, and a `/spacefast:publish` command.

Ask Kimi to "build a landing page and publish it with Spacefast" and you get back a live `*.space.fast` URL. Spaces include a built-in database, versions, sharing, and custom domains.

## What you get

| Component | Name | Purpose |
|---|---|---|
| MCP server | `spacefast` (`https://mcp.spacefast.com`) | Create, publish, update, and share spaces |
| Skill (loaded at session start) | `using-spacefast` | Tells the agent when and how to publish with Spacefast |
| Command | `/spacefast:publish` | Publish the current project, or build and publish what you describe |

## Install

Requires Kimi Code CLI (`npm install -g @moonshot-ai/kimi-code`, then `/login`).

1. Install the plugin:

   ```
   /plugins install https://github.com/jgilmoreburke/spacefast-kimi-code-plugin
   ```

2. Start a fresh session so the skill and MCP server load:

   ```
   /new
   ```

3. Sign in to Spacefast (OAuth). Kimi Code doesn't start this automatically, so run it once:

   ```
   /mcp-config login spacefast
   ```

4. Check it's connected with `/mcp`, and `/plugins info spacefast` for any manifest diagnostics.

## Try it

```
Create a one-page site about local hiking trails and publish it with Spacefast.
```

Or use the command:

```
/spacefast:publish a one-page site for a neighborhood bake sale
```

Kimi asks before each Spacefast tool call. Approve them, and it returns a live URL.

## Troubleshooting

- **Nothing happens after installing.** Plugin changes don't apply to the running session. Run `/reload` or `/new`.
- **Sign-in never opens.** Run `/mcp-config login spacefast` explicitly.
- **Turn the server off.** `/plugins mcp disable spacefast spacefast`, then `/reload`.

## Links

- Spacefast: https://spacefast.com
- Kimi Code plugin docs: https://moonshotai.github.io/kimi-code/en/customization/plugins.html

## License

MIT — see [LICENSE](LICENSE).
