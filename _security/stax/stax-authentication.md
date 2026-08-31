---
api_key_in: []
api_specs:
- filename: stax-api-openapi.json
  format: json
  label: Stax API
  slug: stax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/openapi/stax-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Stax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stax secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stax
provider_slug: stax
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Merchant-level API key. Direct access to Stax Pay for payment processing, invoicing and transaction management; scoped to a single merchant account and cannot reach partner-level functionality.
  level: merchant
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/stax-api-openapi.json
  - https://docs.staxpayments.com/reference/merchant-api-keys
  type: http
- description: Partner-level API key for ISVs and platforms managing many merchants through one integration — merchant creation, enrollment, registration data, per-merchant key issuance and partner-brand webhooks.
  level: partner
  name: PartnerApiKey
  operations_declaring_it: 17
  scheme: bearer
  sources:
  - openapi/stax-api-openapi.json
  - https://docs.staxpayments.com/reference/partner-api-keys
  type: http
- description: Short-lived token minted from an API key by GET /ephemeral. Expires in 24 hours and is used for single sign-on into Stax from a partner surface.
  level: ephemeral
  name: EphemeralAuth
  operations_declaring_it: 2
  scheme: bearer
  sources:
  - openapi/stax-api-openapi.json
  - https://docs.staxpayments.com/reference/ephemeral-authentication-tokens-1
  type: http
slug: stax-authentication
source_filename: stax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.staxpayments.com/reference/overview\ndocs:\n- https://docs.staxpayments.com/reference/overview\n- https://docs.staxpayments.com/reference/merchant-api-keys\n- https://docs.staxpayments.com/reference/partner-api-keys\n- https://docs.staxpayments.com/docs/accessing-and-creating-api-keys\n- https://docs.staxpayments.com/reference/ephemeral-authentication-tokens-1\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: Bearer API key only. No OAuth 2.0, no OIDC, no scope surface — scopes/ is intentionally not emitted.\ntransport:\n  header: Authorization\n  format: Bearer <API key>\n  content_type: application/json\n  tls: TLS 1.2 or 1.3 required; SSLv2/v3 and TLS 1.0/1.1 are blocked at the network level. Certificate and cipher pinning\n    are explicitly discouraged.\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  level: merchant\n\
  \  description: Merchant-level API key. Direct access to Stax Pay for payment processing, invoicing and transaction management;\n    scoped to a single merchant account and cannot reach partner-level functionality.\n  sources:\n  - openapi/stax-api-openapi.json\n  - https://docs.staxpayments.com/reference/merchant-api-keys\n- name: PartnerApiKey\n  type: http\n  scheme: bearer\n  level: partner\n  description: Partner-level API key for ISVs and platforms managing many merchants through one integration — merchant creation,\n    enrollment, registration data, per-merchant key issuance and partner-brand webhooks.\n  operations_declaring_it: 17\n  sources:\n  - openapi/stax-api-openapi.json\n  - https://docs.staxpayments.com/reference/partner-api-keys\n- name: EphemeralAuth\n  type: http\n  scheme: bearer\n  level: ephemeral\n  description: Short-lived token minted from an API key by GET /ephemeral. Expires in 24 hours and is used for single sign-on\n    into Stax from a partner surface.\n\
  \  operations_declaring_it: 2\n  sources:\n  - openapi/stax-api-openapi.json\n  - https://docs.staxpayments.com/reference/ephemeral-authentication-tokens-1\nsandbox_vs_live: Same base URL and same header for both. A sandbox key is bound to a test gateway; a live key processes real\n  money. There is no key PREFIX documented that lets an integrator tell a test key from a live key by inspection — the only\n  published signal is which account issued it.\nclient_side:\n  library: Stax.js\n  credential: Web Payments token (public key)\n  note: Browser tokenization uses a separate public Web Payments token, never the secret API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/authentication/stax-authentication.yml
summary_line: http · 3 schemes
tags:
- Payments
- Payment Processing
- Merchant Services
- Embedded Payments
- ACH
- Invoicing
- Subscription Billing
- Surcharging
- Point-of-Sale
- Tokenization
- Financial-Services
- Fintech
- Card Present
- Merchant Onboarding
---
