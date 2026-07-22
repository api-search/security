---
api_key_in: []
api_specs:
- filename: puzzle-openapi-original.json
  format: json
  label: Puzzle Accounting API
  slug: puzzle-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Puzzle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Puzzle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Puzzle
provider_slug: puzzle
scheme_count: 1
schemes:
- authorizationUrl: https://api.puzzle.io/oauth/authorize
  credentials:
  - client_id
  - client_secret
  - connection_key
  flow: authorizationCode
  name: OAuth2
  pkce: true
  refresh: refresh_token grant supported; offline_access scope for long-lived access
  sandbox_authorizationUrl: https://staging.southparkdata.com/oauth/authorize
  sandbox_tokenUrl: https://staging.southparkdata.com/oauth/token
  scheme: oauth2
  tokenUrl: https://api.puzzle.io/oauth/token
  token_endpoint_auth: Clients may authenticate at the token endpoint via HTTP Basic (recommended for confidential clients) or by including client_id / client_secret in the x-www-form-urlencoded body.
  type: oauth2
slug: puzzle-authentication
source_filename: puzzle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://puzzle-api.readme.io/docs/getting-started\ndocs: https://puzzle-api.readme.io/docs/getting-started\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  legacy: link-token (deprecated)\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: oauth2\n  flow: authorizationCode\n  pkce: true\n  authorizationUrl: https://api.puzzle.io/oauth/authorize\n  tokenUrl: https://api.puzzle.io/oauth/token\n  sandbox_authorizationUrl: https://staging.southparkdata.com/oauth/authorize\n  sandbox_tokenUrl: https://staging.southparkdata.com/oauth/token\n  token_endpoint_auth: >-\n    Clients may authenticate at the token endpoint via HTTP Basic (recommended for\n    confidential clients) or by including client_id / client_secret in the\n    x-www-form-urlencoded body.\n  credentials:\n  - client_id\n  - client_secret\n  - connection_key\n  refresh: refresh_token grant supported; offline_access scope for long-lived\
  \ access\nnotes: >-\n  Authentication is OAuth 2.0 Authorization Code flow with PKCE. Partners request a\n  client ID, client secret, and connection key from Puzzle (api@puzzle.io) and register\n  valid redirect URIs. A legacy link-token flow exists for existing partners but is\n  deprecated in favor of OAuth. The current user can be identified via the /me endpoint,\n  valid only for OAuth connections. The OpenAPI document does not declare securitySchemes;\n  this profile is captured from the developer documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/authentication/puzzle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Accounting
- Financial
- Bookkeeping
- Fintech
- General Ledger
- Payroll
- Agent-Native
- MCP
---
