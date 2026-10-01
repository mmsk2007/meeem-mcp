# Meeem MCP integration

Build and edit Meeem websites, apps and browser games, inspect quota and manage owned app visibility.

Published by Dello AI FZC through its existing maintainer account, `mmsk2007`. This repository contains public integration configuration and workflow instructions only. Product source code and customer data are separate.

## Gemini CLI

```sh
gemini extensions install https://github.com/mmsk2007/meeem-mcp
```

Start Gemini CLI and run `/mcp auth meeem`. Sign in to your own Meeem account and select permissions in the product's OAuth consent screen. The extension uses Streamable HTTP and OAuth discovery with PKCE. No shared API key, client secret or embedded account is included. Your MCP account authentication is separate from Gemini model authentication.

## Grok Build

Use this repository as a plugin source, or install `meeem` from the xAI official marketplace after its catalog submission is accepted. `.grok-plugin/plugin.json`, `.mcp.json`, and `skills/` are included. Marketplace acceptance is not guaranteed by repository publication.

## Consumer Gemini and Grok

Where the account exposes custom MCP apps/connectors, use `https://www.meeem.ai/mcp` and complete the normal OAuth sign-in. A custom account connection is separate from a public consumer app catalog listing. Gemini currently restricts custom apps by account eligibility and region. This repository does not claim consumer catalog approval.

## Permissions, pricing and endpoints

Only `https://www.meeem.ai/mcp` and the OAuth authorization server advertised by that origin are configured. User data stays scoped to the signed-in product account and the permissions selected during consent. No shell commands, hooks, telemetry, account tokens or local secret readers are shipped.

All products have a free version. Plans, credits and connected third-party services may impose limits or charges; this wrapper buys nothing and changes no plan. Meeem Quick builds consume one included Build Credit; Studio consumes five and requires an explicitly requested eligible Pro plan. Hosted app links are accessible to anyone with the link; community publication is a separate action.

Product website: https://www.meeem.ai

Connection guide: https://app.lifemaster.ai/mcp-review/meeem-connection-guide.html

Demo: https://app.lifemaster.ai/mcp-review/meeem-demo.mp4

## License

This wrapper's configuration and instructions are MIT licensed. Product services, product trademarks and remote data remain subject to their own terms and privacy policies.
