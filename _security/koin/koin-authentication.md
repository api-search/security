---
api_key_in:
- header
api_specs:
- filename: koin-access-api-openapi.yml
  format: yaml
  label: Koin Access API
  slug: koin-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-access-api-openapi.yml
- filename: koin-account-take-over-services-api-openapi.yml
  format: yaml
  label: Koin Account Take Over Services API
  slug: koin-account-take-over-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-account-take-over-services-api-openapi.yml
- filename: koin-availability-services-api-openapi.yml
  format: yaml
  label: Koin Availability Services API
  slug: koin-availability-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-availability-services-api-openapi.yml
- filename: koin-communication-services-api-openapi.yml
  format: yaml
  label: Koin Communication Services API
  slug: koin-communication-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-communication-services-api-openapi.yml
- filename: koin-ecommerce-api-openapi.yml
  format: yaml
  label: Koin Ecommerce API
  slug: koin-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-ecommerce-api-openapi.yml
- filename: koin-notification-services-sales-api-openapi.yml
  format: yaml
  label: Koin Notification Services Sales API
  slug: koin-notification-services-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-notification-services-sales-api-openapi.yml
- filename: koin-onboarding-services-api-openapi.yml
  format: yaml
  label: Koin Onboarding Services API
  slug: koin-onboarding-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-onboarding-services-api-openapi.yml
- filename: koin-payment-service-provider-api-openapi.yml
  format: yaml
  label: Koin Payment Service Provider API
  slug: koin-payment-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payment-service-provider-api-openapi.yml
- filename: koin-payment-services-api-openapi.yml
  format: yaml
  label: Koin Payment Services API
  slug: koin-payment-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payment-services-api-openapi.yml
- filename: koin-paymentrequest-api-openapi.yml
  format: yaml
  label: Koin PaymentRequest API
  slug: koin-paymentrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-paymentrequest-api-openapi.yml
- filename: koin-payout-services-api-openapi.yml
  format: yaml
  label: Koin Payout Services API
  slug: koin-payout-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payout-services-api-openapi.yml
- filename: koin-recipient-services-account-api-openapi.yml
  format: yaml
  label: Koin Recipient Services Account API
  slug: koin-recipient-services-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-recipient-services-account-api-openapi.yml
- filename: koin-refund-services-api-openapi.yml
  format: yaml
  label: Koin Refund Services API
  slug: koin-refund-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-refund-services-api-openapi.yml
- filename: koin-support-services-api-openapi.yml
  format: yaml
  label: Koin Support Services API
  slug: koin-support-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-support-services-api-openapi.yml
- filename: koin-tokenize-services-api-openapi.yml
  format: yaml
  label: Koin Tokenize Services API
  slug: koin-tokenize-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-tokenize-services-api-openapi.yml
- filename: koin-wiretransfer-api-openapi.yml
  format: yaml
  label: Koin WireTransfer API
  slug: koin-wiretransfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-wiretransfer-api-openapi.yml
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
- Financial-Services
- Brazil
- Latin America
- Anti-Fraud
- Checkout
- Company
---
