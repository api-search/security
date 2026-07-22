---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Montonio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Montonio secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Montonio
provider_slug: montonio
scheme_count: 2
schemes:
- algorithm: HS256
  api: Montonio Payments API (Stargate)
  bearer_format: JWT
  name: StargatePostJWT
  placement: GET endpoints send the signed JWT in the Authorization header. POST endpoints send the JWT AS the request payload (the token itself contains the request data), with the minimum payload {accessKey, exp}.
  required_claims:
  - accessKey
  - exp
  scheme: bearer
  source: docs
  type: http
- algorithm: HS256
  api: Montonio Shipping API (v2)
  bearer_format: JWT
  name: ShippingBearerJWT
  placement: All endpoints require the JWT in the Authorization header as a Bearer token.
  required_claims:
  - accessKey
  - exp
  scheme: bearer
  source: docs
  type: http
slug: montonio-authentication
source_filename: montonio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.montonio.com/api/stargate/reference#authentication\ndocs:\n- https://docs.montonio.com/api/stargate/reference#authentication\n- https://docs.montonio.com/api/shipping-v2/reference#authentication\n- https://docs.montonio.com/introduction#api-keys\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  algorithm: HS256\n  credential_source: Partner System store API keys (Access Key + Secret Key)\n  key_environments: [sandbox, production]\nnotes: >-\n  Both Montonio APIs authenticate with JSON Web Tokens (JWT) signed with the\n  store Secret Key using HMAC SHA256 (HS256); every token must carry the store\n  Access Key. There is no OAuth2 client-credentials or scope surface, so no\n  scopes/ artifact applies. Keys are issued per store under Partner System ->\n  Stores -> API Keys, separately for the Sandbox and Production environments;\n  generating new keys invalidates the old ones.\nschemes:\n- name:\
  \ StargatePostJWT\n  api: Montonio Payments API (Stargate)\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  algorithm: HS256\n  placement: >-\n    GET endpoints send the signed JWT in the Authorization header. POST endpoints\n    send the JWT AS the request payload (the token itself contains the request\n    data), with the minimum payload {accessKey, exp}.\n  required_claims: [accessKey, exp]\n  source: docs\n- name: ShippingBearerJWT\n  api: Montonio Shipping API (v2)\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  algorithm: HS256\n  placement: All endpoints require the JWT in the Authorization header as a Bearer token.\n  required_claims: [accessKey, exp]\n  source: docs\nconnect_flow:\n  name: Connect Montonio (for plugins)\n  description: >-\n    An OAuth-like authorization flow for plugin/platform partners: the merchant\n    is sent to the Montonio Partner System to consent, a state parameter guards\n    against CSRF, and a short-lived single-use one-time code is\
  \ exchanged\n    server-to-server for the store API keys.\n  docs: https://docs.montonio.com/api/stargate/guides\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montonio/refs/heads/main/authentication/montonio-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Payments
- Payment Processing
- Open Banking
- E-commerce
- Shipping
- Logistics
- Financing
- Baltics
- Webhooks
- SDK
---
