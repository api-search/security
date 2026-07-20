---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Common Paper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Common Paper secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Common Paper
provider_slug: common-paper
scheme_count: 1
schemes:
- description: Production API token. Generate from the account Integrations tab at app.commonpaper.com, or obtain via the agentic provisioning flow. The org is inferred from the token.
  format: Bearer <API token>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  token_prefix: zpka_
  type: http
slug: common-paper-authentication
source_filename: common-paper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.commonpaper.com/docs/authentication\ndocs: https://api.commonpaper.com/docs/authentication\nnote: >-\n  Common Paper's REST API and hosted MCP server both use Bearer-token\n  authentication. A single API token is supplied in the Authorization header; the\n  organization is inferred from the token (no organization-id header). Tokens are\n  generated from the account Integrations tab or minted programmatically via the\n  agentic provisioning flow. The end-user web application (app.commonpaper.com)\n  is fronted by Auth0. The API is served through a Zuplo gateway (token prefix\n  zpka_).\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API token>'\n  token_prefix: zpka_\n  description: >-\n    Production API token. Generate from the account Integrations\
  \ tab at\n    app.commonpaper.com, or obtain via the agentic provisioning flow. The org is\n    inferred from the token.\nprovisioning:\n  description: >-\n    Two unauthenticated public gateway endpoints support agentic signup: mint a\n    single-use provision key, then redeem it for a new organization + admin user\n    and receive a production API key.\n  endpoints:\n  - POST /v1/keys      # mint a one-time provision key (contact_email required)\n  - POST /v1/accounts  # redeem provision key -> new org + production api_key\n  rate_limits: 5 req/minute, 50 req/day per IP (provision key minting)\napp_login:\n  provider: Auth0\n  signup: https://app.commonpaper.com/auth/auth0?screen_hint=signup\n  signin: https://app.commonpaper.com/auth/auth0?screen_hint=signin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-paper/refs/heads/main/authentication/common-paper-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Contracts
- Contract Management
- Legal Tech
- Agreements
- SaaS Contracts
- E-Signature
- API
- Webhooks
- MCP
---
