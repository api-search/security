---
api_key_in:
- header
api_specs:
- filename: super-payments-openapi.yml
  format: yaml
  label: Super Payments API
  slug: super-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-openapi.yml
auth_types:
- apiKey
description: 'Super Payments authenticates server-side requests with a static secret API key passed raw in the Authorization header (no Bearer prefix). Two key types exist: secret keys (sk_prod_ / sk_test_) for server-side use, and public keys (PUB_) safe for client-side/front-end use. There is no OAuth2/OIDC. Webhooks are authenticated separately via an HMAC-SHA256 super-signature header. All calls must be over HTTPS.'
kind: authentication
layout: security
method: searched
name: Super Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Super Payments secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Super Payments
provider_slug: super-payments
scheme_count: 2
schemes:
- description: Merchant API key
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/super-payments-openapi.yml
  type: apiKey
- description: Header used to validate the webhook request
  in: header
  name: HMAC
  parameter: super-signature
  sources:
  - openapi/super-payments-openapi.yml
  type: apiKey
slug: super-payments-authentication
source_filename: super-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/super-payments-openapi.yml\ndocs: https://docs.superpayments.com/reference/authentication\ndescription: >-\n  Super Payments authenticates server-side requests with a static secret API key\n  passed raw in the Authorization header (no Bearer prefix). Two key types exist:\n  secret keys (sk_prod_ / sk_test_) for server-side use, and public keys (PUB_)\n  safe for client-side/front-end use. There is no OAuth2/OIDC. Webhooks are\n  authenticated separately via an HMAC-SHA256 super-signature header. All calls\n  must be over HTTPS.\nkey_types:\n  - {name: secret, prefixes: [sk_prod_, sk_test_], usage: server-side, header: Authorization}\n  - {name: public, prefixes: [PUB_], usage: client-side / front-end}\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Merchant API key\n  sources:\n  - openapi/super-payments-openapi.yml\n\
  - name: HMAC\n  type: apiKey\n  in: header\n  parameter: super-signature\n  description: Header used to validate the webhook request\n  sources:\n  - openapi/super-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/authentication/super-payments-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Open Banking
- Cash Rewards
- Checkout
- Fintech
- United Kingdom
- Pay by Bank
---
