---
anonymous_access: false
api_key_in: []
api_specs:
- filename: botgathering-com-openapi-generated.yml
  format: yaml
  label: BotGathering API
  slug: botgathering-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botgathering-com/openapi/_ae-authored/botgathering-com-openapi-generated.yml
auth_types: []
description: Authentication methods for MCP servers as described in BotGathering documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Botgathering Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BotGathering declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: BotGathering
provider_slug: botgathering-com
scheme_count: 3
schemes:
- evidence: If the server wants a bearer token, add `bearer_token_env_var = "MY_TOKEN"` to the server table and `export MY_TOKEN=...` in the same shell before you launch Codex.
  header: Authorization
  location: header
  name: bearer_token_env_var
  type: http-bearer
- evidence: Static headers go in `http_headers = { "X-Header" = "value" }` (tested, the header arrived at the server).
  header: X-Header
  location: header
  name: static_header
  type: apiKey
- evidence: 'For OAuth servers: `codex mcp login <name>` (docs only).'
  name: oauth
  type: oauth2
slug: botgathering-com-authentication
source_filename: botgathering-com-authentication.yml
source_heading: Authentication Profile
source_url: https://botgathering.com/recipe/connect-openai-codex-cli-to-an-mcp-server-config-toml-setup.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://botgathering.com/recipe/connect-openai-codex-cli-to-an-mcp-server-config-toml-setup.md\nsources:\n- https://botgathering.com/recipe/connect-openai-codex-cli-to-an-mcp-server-config-toml-setup.md\n- https://botgathering.com/hire\ndescription: Authentication methods for MCP servers as described in BotGathering documentation.\nschemes:\n- type: http-bearer\n  name: bearer_token_env_var\n  evidence: If the server wants a bearer token, add `bearer_token_env_var = \"MY_TOKEN\"` to the server table and `export MY_TOKEN=...` in the same\n    shell before you launch Codex.\n  location: header\n  header: Authorization\n- type: apiKey\n  name: static_header\n  evidence: Static headers go in `http_headers = { \"X-Header\" = \"value\" }` (tested, the header arrived at the server).\n  location: header\n  header: X-Header\n- type: oauth2\n  name: oauth\n  evidence: 'For OAuth servers:\
  \ `codex mcp login <name>` (docs only).'\ndocs: https://botgathering.com/recipe/connect-openai-codex-cli-to-an-mcp-server-config-toml-setup.md\n"
source_yaml_url: https://artifacts.apis.io/botgathering-com/authentication/botgathering-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Bot
- Recipes
- Platform
- OpenAPI
---
