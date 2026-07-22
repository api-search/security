---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Synthetic Sciences Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: Synthetic Sciences secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: Synthetic Sciences
provider_slug: synthetic-sciences
scheme_count: 2
schemes:
- description: 'Atlas API keys are prefixed `thk_` and sent as `Authorization: Bearer <key>`. Minted with `atlas key:create` or in the app; the full secret is shown once. Managed via /api/v1/auth/api-keys (create/list/rotate/delete). Intended for agents, scripts, and CI. Supports `--expiry-days` for short-lived automation.'
  header: 'Authorization: Bearer thk_...'
  management_routes:
  - method: POST
    route: /auth/api-keys
    use: create
  - method: GET
    route: /auth/api-keys
    use: list
  - method: POST
    route: /auth/api-keys/{key_id}/rotate
    use: rotate
  - method: DELETE
    route: /auth/api-keys/{key_id}
    use: revoke
  name: BearerToken
  scheme: bearer
  type: http
- description: 'Interactive human login: `atlas login` starts a localhost callback, opens the Atlas approval page, redeems a one-time token, and writes an API key to the active local profile (file mode 0600). Both auth paths resolve to a `thk_*` key sent as a bearer token. The legacy MCP-era device-pairing and token-exchange flows are retired and now return HTTP 426 Upgrade Required.'
  flow: interactive-browser
  name: BrowserLogin
  routes:
  - method: POST
    route: /auth/cli/browser/start
    use: start browser login
  - method: GET
    route: /auth/status
    use: verify auth
  type: oauth2
slug: synthetic-sciences-authentication
source_filename: synthetic-sciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.syntheticsciences.ai/atlas/authentication\ndocs: https://docs.syntheticsciences.ai/atlas/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  api_key_prefix: thk_\n  oauth2_flows: [browser-login]\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Atlas API keys are prefixed `thk_` and sent as `Authorization: Bearer <key>`.\n      Minted with `atlas key:create` or in the app; the full secret is shown once.\n      Managed via /api/v1/auth/api-keys (create/list/rotate/delete). Intended for\n      agents, scripts, and CI. Supports `--expiry-days` for short-lived automation.\n    header: \"Authorization: Bearer thk_...\"\n    management_routes:\n      - {method: POST, route: \"/auth/api-keys\", use: create}\n      - {method: GET, route: \"/auth/api-keys\", use: list}\n      - {method: POST, route: \"/auth/api-keys/{key_id}/rotate\", use: rotate}\n\
  \      - {method: DELETE, route: \"/auth/api-keys/{key_id}\", use: revoke}\n  - name: BrowserLogin\n    type: oauth2\n    flow: interactive-browser\n    description: >-\n      Interactive human login: `atlas login` starts a localhost callback, opens the\n      Atlas approval page, redeems a one-time token, and writes an API key to the\n      active local profile (file mode 0600). Both auth paths resolve to a `thk_*`\n      key sent as a bearer token. The legacy MCP-era device-pairing and token-exchange\n      flows are retired and now return HTTP 426 Upgrade Required.\n    routes:\n      - {method: POST, route: /auth/cli/browser/start, use: start browser login}\n      - {method: GET, route: /auth/status, use: verify auth}\nconfig_resolution:\n  order: [\"--api-key <key>\", \"ATLAS_API_KEY env\", \"active profile (atlas login)\", \"root config fallback\"]\n  env_vars: [ATLAS_API_KEY, ATLAS_BASE_URL, ATLAS_CLI_CONFIG_PATH, ATLAS_LOGIN_TIMEOUT_MS]\n  storage: \"local profile file (0600) or\
  \ macOS Keychain (atlas secret:set)\"\nintegrations:\n  - {name: GitHub, method: OAuth app install or PAT, routes: [/auth/github/install-url, /auth/github/pat, /auth/github/status]}\n  - {name: HuggingFace, method: access token, routes: [/auth/integrations/huggingface]}\n  - {name: \"Weights & Biases\", method: API key, routes: [/auth/integrations/wandb]}\nnotes: >-\n  No OpenAPI/Swagger document is published (the docs expose route tables, not a machine\n  spec), so this profile is searched from the official auth docs rather than derived.\n  Auth is bearer-key based; there is no documented OAuth scope surface, so no scopes/ artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthetic-sciences/refs/heads/main/authentication/synthetic-sciences-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Scientific Research
- Developer Tools
- Agents
- Foundation Models
- Knowledge Graph
- Model Context Protocol
- CLI
- Research Infrastructure
---
