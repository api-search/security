---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: PageAudit API
  slug: pageaudit-api
  spec_type: OpenAPI
  url: https://pageaudit.online/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pageaudit Authentication
name_suffix: Authentication
oauth_flows: []
overview: PageAudit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PageAudit
provider_slug: pageaudit
scheme_count: 1
schemes:
- description: 'Guest token (`POST /api/guest`) in `X-Guest-Token: pa_…`, `Authorization: Bearer pa_…` or `?guest_token=pa_…`. A user session (`sess_…`) also works and takes precedence.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pageaudit-openapi.json
  type: http
slug: pageaudit-authentication
source_filename: pageaudit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: openapi/pageaudit-openapi.json\ndocs: https://pageaudit.online/api/\nnote: >-\n  Derived from the OpenAPI securitySchemes, then upgraded from the self-describing API index\n  (GET https://pageaudit.online/api/, fetched 2026-09-07), which documents four auth modes the\n  single bearerAuth scheme multiplexes. No OAuth; no API-key portal — tokens are minted by the\n  API itself (POST /api/guest, POST /api/auth/verify) or by an x402 payment (POST /api/credito).\nsummary:\n  types:\n    - http\n  modes:\n    - none\n    - guest\n    - session\n    - credito\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Guest token (`POST /api/guest`) in `X-Guest-Token: pa_…`, `Authorization: Bearer pa_…` or\n      `?guest_token=pa_…`. A user session (`sess_…`) also works and takes precedence.\n    sources:\n      - openapi/pageaudit-openapi.json\nmodes:\n  - mode: none\n    description: Public, no\
  \ credential — discovery, one-shot audit, micro-tools, billing, gate, metrics.\n  - mode: guest\n    description: >-\n      Guest token `pa_…` from POST /api/guest; sent as `X-Guest-Token`, `Authorization: Bearer pa_…`\n      or `?guest_token=`. Grants the persistent tab workspace without an account.\n  - mode: session\n    description: >-\n      User session `sess_…` via e-mail code (POST /api/auth/start → POST /api/auth/verify);\n      `Authorization: Bearer sess_…`. Takes precedence over a guest token. Confirming the e-mail\n      grants a 90-day full-access trial.\n  - mode: credito\n    description: >-\n      Prepaid credit token `cred_…` (topped up once via x402 at POST /api/credito) in\n      `Authorization: Bearer cred_…` or the `X-Credito` header. A bearer of balance, not an account.\npayment:\n  scheme: x402\n  description: >-\n    Past the free allowance the API answers HTTP 402 with `accepts[]` (USDC on Base, chain 8453);\n    pay and repeat the same call with the `X-PAYMENT`\
  \ header. Humans clear Turnstile instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pageaudit/refs/heads/main/authentication/pageaudit-authentication.yml
summary_line: http · 1 scheme
tags:
- Technical SEO
- SEO auditing
- Developer Tools
- Agent-native
- MCP
- x402
---
