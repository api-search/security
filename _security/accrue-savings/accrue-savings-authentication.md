---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accrue-savings-merchant-api-openapi.yaml
  format: yaml
  label: Accrue Merchant API
  slug: accrue-savings-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-merchant-api-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accrue Savings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accrue Savings declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Accrue Savings
provider_slug: accrue-savings
scheme_count: 2
schemes:
- description: 'Every API call carries `Authorization: Bearer <Client Secret>`. The Client Secret is issued per Client (merchant) and is a backend-only credential — the docs state it must never appear in client-side code and should be rotated periodically. An invalid, missing, or expired token returns HTTP 401.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  source: https://docs.byaccrue.com/api/
  type: http
- description: A Client-ID header accompanies the bearer token and identifies the merchant tenant. It is declared as a required header parameter on all 82 operations in the OpenAPI.
  in: header
  name: clientId
  parameter: Client-ID
  source: openapi/accrue-savings-merchant-api-openapi.yaml
  type: apiKey
slug: accrue-savings-authentication
source_filename: accrue-savings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.byaccrue.com/api/ (Introduction > Authentication) and https://docs.byaccrue.com/getting-started-api\ndocs: https://docs.byaccrue.com/api/\nsummary: Bearer token (the Client Secret) plus a Client-ID header, sent on every request. There is no\n  OAuth, no OIDC, and no mTLS.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: 'Every API call carries `Authorization: Bearer <Client Secret>`. The Client Secret is issued\n    per Client (merchant) and is a backend-only credential — the docs state it must never appear in client-side\n    code and should be rotated periodically. An invalid, missing, or expired token returns HTTP 401.'\n  source: https://docs.byaccrue.com/api/\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: Client-ID\n  description: A Client-ID header accompanies the bearer token and identifies the merchant tenant. It\n   \
  \ is declared as a required header parameter on all 82 operations in the OpenAPI.\n  source: openapi/accrue-savings-merchant-api-openapi.yaml\noauth2: false\nopenid_connect: false\nmutual_tls: false\nerrors:\n  '401': Unauthorized — token invalid, missing, or expired\n  '403': ForbiddenException — observed live on an unauthenticated GET /api/v1/payments\ngaps:\n- The OpenAPI declares NO components.securitySchemes and no top-level or per-operation `security` block.\n  Authentication is expressed only as two required header parameters (Authorization, Client-ID) on each\n  operation, plus prose in the Introduction section. A generator or agent reading the spec alone cannot\n  tell that these are credentials, which is why derive-authentication.py produced nothing for this provider\n  and this file was written from the docs instead.\n- No credential-rotation endpoint, no token expiry semantics, and no scope model are published.\nwebhook_auth:\n  mechanism: signature verification\n  note: The\
  \ getting-started guide instructs integrators to verify webhook signatures with a constant-time\n    comparison, but the signing header name and algorithm are not published in the public docs or the\n    OpenAPI.\n  source: https://docs.byaccrue.com/getting-started-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/authentication/accrue-savings-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Loyalty
- Wallets
- Stored Value
- Rewards
- Banking
- Fintech
- Webhooks
---
