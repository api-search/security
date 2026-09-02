---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Paymentus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paymentus secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paymentus
provider_slug: paymentus
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: XOTP payment calls carry a short-lived Bearer JWT in the Authorization header. The token is minted by the Auth API (@paymentus/auth) from a pre-shared key identified by a key id (kid) and a three-letter application acronym (tla), optionally an audience (aud, e.g. WEB_SDK), and the set of granular scopes (or a Paymentus "pixel" that maps to scopes) the client needs. See scopes/paymentus-scopes.yml for the scope catalog.
  name: BearerAuth
  scheme: bearer
  sources:
  - packages/paymentus-packages.yml
  type: http
slug: paymentus-authentication
source_filename: paymentus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://www.npmjs.com/package/@paymentus/auth\ndocs: https://developer.paymentus.io/\nsummary:\n  types: [http, oauth2]\n  scheme: bearer\n  bearer_format: JWT\n  token_issuance: pre-shared-key signed request\n  oauth2_style_scopes: true\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      XOTP payment calls carry a short-lived Bearer JWT in the Authorization\n      header. The token is minted by the Auth API (@paymentus/auth) from a\n      pre-shared key identified by a key id (kid) and a three-letter application\n      acronym (tla), optionally an audience (aud, e.g. WEB_SDK), and the set of\n      granular scopes (or a Paymentus \"pixel\" that maps to scopes) the client\n      needs. See scopes/paymentus-scopes.yml for the scope catalog.\n    sources: [packages/paymentus-packages.yml]\nsession_headers:\n  - name: X-Ext-Session-Id\n    description: Per-session\
  \ UUID sent alongside the Bearer token on XOTP calls.\n  - name: X-Ext-Session-App\n    description: Client application identifier (e.g. xotp-sdk@1.0.0).\nnotes: >-\n  No anonymous OIDC/OAuth discovery document was served on the API host\n  (/.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  return no response on api.paymentus.com). The token endpoint and full auth\n  reference sit behind the developer.paymentus.io request-access gate; the model\n  above is documented publicly through the @paymentus/auth SDK README.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymentus/refs/heads/main/authentication/paymentus-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Payments
- United States
- Bill Payments
- Electronic Bill Presentment
- Payment Processing
- Payment Gateway
- Disbursements
- ACH
- Real-Time Payments
- Tokenization
---
