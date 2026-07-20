---
api_key_in:
- header
api_specs:
- filename: koin-payments-openapi.json
  format: json
  label: Koin Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payments-openapi.json
- filename: koin-antifraud-evaluations-openapi.json
  format: json
  label: Koin Antifraud API
  slug: antifraud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-antifraud-evaluations-openapi.json
- filename: koin-onboarding-openapi.json
  format: json
  label: Koin Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-onboarding-openapi.json
- filename: koin-bnpl-openapi.json
  format: json
  label: Koin BNPL Payment Request API
  slug: bnpl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-bnpl-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Koin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Koin
provider_slug: koin
scheme_count: 2
schemes:
- applies_to:
  - openapi/koin-payments-openapi.json
  - openapi/koin-antifraud-evaluations-openapi.json
  - openapi/koin-antifraud-ecommerce-openapi.json
  - openapi/koin-antifraud-lifecycle-openapi.json
  - openapi/koin-antifraud-wire-transfer-openapi.json
  - openapi/koin-antifraud-ato-openapi.json
  - openapi/koin-onboarding-openapi.json
  description: Koin private key sent as a bearer credential, format `sk_` + 32 alphanumeric characters.
  docs: https://api-docs.koin.com.br/docs/security-scheme
  name: PrivateKey
  parameter: Authorization
  scheme: bearer
  type: http
- description: Authorization header declared in the BNPL Payment Request contract; carries the token minted by the Generate Authorization Token operation.
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/koin-bnpl-openapi.json
  type: apiKey
slug: koin-authentication
source_filename: koin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api-docs.koin.com.br/docs/security-scheme\ndocs: https://api-docs.koin.com.br/docs/security-scheme\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: single private key (bearer-style) shared across every Koin API — payments, antifraud and BNPL\n  key_issuance: issued by the Koin team as part of merchant onboarding; not self-service\nnotes:\n- Koin documents one credential for the whole platform. A client/store needs only the private key to\n  reach payments, antifraud and BNPL services.\n- The private key is sent in the HTTP Authorization header as `Authorization: Bearer <private key>`.\n- Documented key format is a fixed `sk_` prefix followed by a 32-character mixed-case alphanumeric\n  string.\n- The BNPL Payment Request API additionally exposes a token-minting operation\n  (`generate-by-rest`, POST /access/token/resource) that returns an authorization token used by the\n  `check`\
  \ and `include` operations on the legacy sp-api host.\n- No OAuth 2.0 or OpenID Connect surface is documented; `scopes/` is intentionally not produced.\nschemes:\n- name: PrivateKey\n  type: http\n  scheme: bearer\n  parameter: Authorization\n  description: Koin private key sent as a bearer credential, format `sk_` + 32 alphanumeric characters.\n  docs: https://api-docs.koin.com.br/docs/security-scheme\n  applies_to:\n  - openapi/koin-payments-openapi.json\n  - openapi/koin-antifraud-evaluations-openapi.json\n  - openapi/koin-antifraud-ecommerce-openapi.json\n  - openapi/koin-antifraud-lifecycle-openapi.json\n  - openapi/koin-antifraud-wire-transfer-openapi.json\n  - openapi/koin-antifraud-ato-openapi.json\n  - openapi/koin-onboarding-openapi.json\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header declared in the BNPL Payment Request contract; carries the token\n    minted by the Generate Authorization Token operation.\n  sources:\n\
  \  - openapi/koin-bnpl-openapi.json\nclient_side:\n- name: clientKey\n  used_by: Koin Checkout SDK (browser tokenization)\n  description: Publishable client key used to initialize the browser tokenization SDK; distinct from\n    the server-side private key.\n  docs: https://api-docs.koin.com.br/reference/koin-checkout-sdk\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/authentication/koin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- Fraud Prevention
- Buy Now Pay Later
- Pix
- E-Commerce
- Financial Services
- Brazil
- Latin America
- Anti-Fraud
- Checkout
- Company
---
