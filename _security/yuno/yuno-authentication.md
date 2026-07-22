---
api_key_in:
- header
api_specs:
- filename: yuno-openapi-original.json
  format: json
  label: Yuno Payments API
  slug: yuno-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuno/refs/heads/main/openapi/yuno-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Yuno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yuno secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yuno
provider_slug: yuno
scheme_count: 3
schemes:
- description: Public API key from the Yuno Dashboard (client/SDK context).
  header: public-api-key
  in: header
  name: publicApiKey
  sources:
  - openapi/yuno-openapi-original.json
  type: apiKey
- description: Private secret key, server-side only.
  header: private-secret-key
  in: header
  name: privateSecretKey
  sources:
  - openapi/yuno-openapi-original.json
  type: apiKey
- alias_header: X-Account-Code
  description: Merchant account identifier.
  header: account-code
  in: header
  name: accountCode
  sources:
  - openapi/yuno-openapi-original.json
  type: apiKey
slug: yuno-authentication
source_filename: yuno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.y.uno/reference/authentication\ndocs: https://docs.y.uno/reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Yuno uses paired header API keys — a public key for client-side/SDK context\n    and a private secret key for server-side calls — plus an account-code header\n    that identifies the merchant account. Sandbox and production use different\n    keys. There is no OAuth2 flow on the core payments API (OAuth2 exists only as\n    an optional authentication mode for outbound webhook delivery). Keys are\n    issued from the Yuno Dashboard (dashboard.y.uno/developers).\nschemes:\n  - name: publicApiKey\n    type: apiKey\n    in: header\n    header: public-api-key\n    description: Public API key from the Yuno Dashboard (client/SDK context).\n    sources: [openapi/yuno-openapi-original.json]\n  - name: privateSecretKey\n    type: apiKey\n    in: header\n\
  \    header: private-secret-key\n    description: Private secret key, server-side only.\n    sources: [openapi/yuno-openapi-original.json]\n  - name: accountCode\n    type: apiKey\n    in: header\n    header: account-code\n    alias_header: X-Account-Code\n    description: Merchant account identifier.\n    sources: [openapi/yuno-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuno/refs/heads/main/authentication/yuno-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Payments
- Payment Orchestration
- Fintech
- Checkout
- Payouts
- Subscriptions
- API
---
