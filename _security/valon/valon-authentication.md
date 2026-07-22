---
api_key_in: []
auth_types:
- http-bearer
- session-cookie
description: ''
kind: authentication
layout: security
method: searched
name: Valon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valon secures its APIs with http-bearer and session-cookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Valon
provider_slug: valon
scheme_count: 2
schemes:
- description: Authenticated routes accept an Authorization Bearer token. Tokens are issued and managed via the token endpoints (POST /api/v1/tokens, DELETE /api/v1/tokens/{id}) and the gestalt CLI token management flows.
  name: bearerToken
  scheme: bearer
  sources:
  - https://gestaltd.ai/reference/http-api
  type: http
- description: Browser sessions authenticate with a session_token cookie set by the login flow.
  in: cookie
  name: sessionToken
  parameter: session_token
  sources:
  - https://gestaltd.ai/reference/http-api
  type: apiKey
slug: valon-authentication
source_filename: valon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://gestaltd.ai/reference/http-api\nsource: https://gestaltd.ai/reference/http-api\nnotes: >-\n  Valon publishes no OpenAPI document, so this profile is captured from the\n  Gestalt HTTP API reference (gestaltd.ai). Gestalt is Valon's open source,\n  self-hostable agentic tools platform; authentication applies to each\n  self-hosted deployment. Valon's consumer mortgage-servicing surfaces\n  (valon.com) expose account login only, with no public API authentication.\nsummary:\n  types: [http-bearer, session-cookie]\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Authenticated routes accept an Authorization Bearer token. Tokens are\n      issued and managed via the token endpoints (POST /api/v1/tokens,\n      DELETE /api/v1/tokens/{id}) and the gestalt CLI token management flows.\n    sources: [https://gestaltd.ai/reference/http-api]\n  - name: sessionToken\n\
  \    type: apiKey\n    in: cookie\n    parameter: session_token\n    description: Browser sessions authenticate with a session_token cookie set by the login flow.\n    sources: [https://gestaltd.ai/reference/http-api]\nunauthenticated_routes:\n  - /health\n  - /ready\n  - /admin\n  - login/logout endpoints\n  - POST /api/v2/identity/authorize\n  - POST /api/v2/identity/token\nidentity_note: >-\n  Identity flows, credential storage, encryption at rest, token refresh, and\n  RBAC are provided through Gestalt's provider ecosystem\n  (https://gestaltd.ai/providers/identity, /providers/authorization).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valon/refs/heads/main/authentication/valon-authentication.yml
summary_line: http-bearer/session-cookie · 2 schemes
tags:
- Company
- Mortgages
- Loan Servicing
- Lending
- Fintech
- Real Estate
- Insurance
- Agentic Tools
- MCP
- Open Source
---
