---
api_key_in:
- header
api_specs:
- filename: aza-finance-openapi-original.json
  format: json
  label: TransferZero API V1
  slug: transferzero-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aza Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: AZA Finance secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AZA Finance
provider_slug: aza-finance
scheme_count: 4
schemes:
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationKey
  parameter: Authorization-Key
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationSecret
  parameter: Authorization-Secret
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationNonce
  parameter: Authorization-Nonce
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
- description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication) on how to use these fields
  in: header
  name: AuthorizationSignature
  parameter: Authorization-Signature
  sources:
  - openapi/aza-finance-openapi-original.json
  type: apiKey
slug: aza-finance-authentication
source_filename: aza-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aza-finance-openapi-original.json\ndocs: https://docs.transferzero.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: hmac\n  detail: >-\n    Two documented modes. Preferred: HMAC request signing using Authorization-Key,\n    Authorization-Nonce and Authorization-Signature headers (signature is an HMAC over\n    the request built from the API secret). Simpler alternative for lower-risk calls:\n    Authorization-Key + Authorization-Secret. Sandbox and production use separate\n    key/secret pairs. Webhook callbacks are signed with the same HMAC scheme.\nschemes:\n- name: AuthorizationKey\n  type: apiKey\n  in: header\n  parameter: Authorization-Key\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationSecret\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization-Secret\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationNonce\n  type: apiKey\n  in: header\n  parameter: Authorization-Nonce\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n- name: AuthorizationSignature\n  type: apiKey\n  in: header\n  parameter: Authorization-Signature\n  description: Please see the [Authentication guide](https://docs.transferzero.com/docs/authentication)\n    on how to use these fields\n  sources:\n  - openapi/aza-finance-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/authentication/aza-finance-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Financial Services
- Payments
- Foreign Exchange
- Cross-Border Payments
- Africa
- Fintech
- API
---
