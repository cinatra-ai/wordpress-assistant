# WordPress

The Cinatra WordPress authoring assistant — an agent-kind assistant extension. Its `cinatra/config.json` declares the assistant: a WordPress authoring persona, the WordPress authoring skill bundle, a remote launch that opens the connected site's `wp-admin`, and webhook turn delivery. It handles no credentials of its own — every WordPress call resolves through the `@cinatra-ai/wordpress-assistant-connector` it depends on.

## Works with

- `@cinatra-ai/wordpress-assistant-connector` — resolves the connected WordPress site and its credentials (required runtime dependency)

## Capabilities

- Drafts, structures, and publishes WordPress content — posts, pages, blocks, categories, tags, and media — against the connected site
- Prefers the WordPress authoring skills and the site's own taxonomy
- Launches remotely into the connected site's `wp-admin` and delivers each turn over a webhook channel
