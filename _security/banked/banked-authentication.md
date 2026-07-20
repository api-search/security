---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Banked Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Banked secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Banked
provider_slug: banked
scheme_count: 1
schemes:
- flow: clientCredentials
  name: OAuth2
  scope_note: The scope value carried by MCP/API clients is the business application ID (BANKED_OAUTH_CLIENT_SCOPE); Banked does not publish a granular OAuth scope reference, so scopes/ is intentionally omitted.
  sources:
  - https://github.com/banked/postman-collections-public
  - https://github.com/banked/example-agents
  token_type: Bearer
  token_url: https://api.banked.com/oauth/token
  type: oauth2
slug: banked-authentication
source_filename: banked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.banked.com/reference\ndocs: https://developer.banked.com/reference\nnotes: >-\n  No public OpenAPI is available to derive from; the auth model was read from\n  the developer reference, the public Partner POC Postman collection, and the\n  MCP configuration. Banked authenticates with OAuth 2.0 client credentials:\n  clients exchange a client_id/client_secret (plus a scope that is the business\n  application ID) for a bearer access token at api.banked.com/oauth/token, then\n  call the API with Authorization: Bearer. The same OAuth server backs the\n  hosted MCP server.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.banked.com/oauth/token\n  token_type: Bearer\n  scope_note: >-\n    The scope value carried by MCP/API clients is the business application ID\n    (BANKED_OAUTH_CLIENT_SCOPE); Banked\
  \ does not publish a granular OAuth scope\n    reference, so scopes/ is intentionally omitted.\n  sources:\n  - https://github.com/banked/postman-collections-public\n  - https://github.com/banked/example-agents\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banked/refs/heads/main/authentication/banked-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Open Banking
- Account-to-Account
- Pay by Bank
- Fintech
- Payment Processing
- Payouts
---
