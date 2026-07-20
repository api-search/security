---
api_key_in:
- authorization-header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Beam Checkout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beam Checkout secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beam Checkout
provider_slug: beam-checkout
scheme_count: 3
schemes:
- base_url: https://api.beamcheckout.com/api/v1/
  header: 'Authorization: Basic base64(merchantId:apiKey)'
  managed_in: Lighthouse dashboard (Developers section)
  name: MerchantApiKey
  password: merchant API key
  scheme: basic
  type: http
  usage: server-side requests
  username: merchantId
- additional_header: 'X-Beam-Partner-ID: {partnerId}'
  base_url: https://api.beamcheckout.com/api/v1/
  managed_in: Bridge (Merchants > API Keys)
  name: PartnerApiKey
  password: partner API key
  scheme: basic
  type: http
  usage: server-side requests by partners on behalf of merchants
  username: merchantId
- base_url: https://api.beamcheckout.com/client/v1/
  name: PublishableKey
  note: publishable key is safe to be shared client-side
  password: publishable key
  scheme: basic
  type: http
  usage: client-side requests to /client endpoints (e.g. card tokenization)
  username: merchantId
slug: beam-checkout-authentication
source_filename: beam-checkout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.beamcheckout.com/get-started/authentication\ndocs: https://docs.beamcheckout.com/get-started/authentication\nsummary:\n  types: [http]\n  http_scheme: basic\n  api_key_in: [authorization-header]\n  oauth2_flows: []\n  note: >-\n    Beam uses HTTP Basic authentication for all API keys. Credentials are the\n    base64 encoding of merchantId:apiKey sent in the Authorization header.\n    Playground and Production keys are separate and cannot be used interchangeably.\nschemes:\n  - name: MerchantApiKey\n    type: http\n    scheme: basic\n    usage: server-side requests\n    username: merchantId\n    password: merchant API key\n    base_url: https://api.beamcheckout.com/api/v1/\n    managed_in: Lighthouse dashboard (Developers section)\n    header: 'Authorization: Basic base64(merchantId:apiKey)'\n  - name: PartnerApiKey\n    type: http\n    scheme: basic\n    usage: server-side requests by partners on behalf of merchants\n\
  \    username: merchantId\n    password: partner API key\n    additional_header: 'X-Beam-Partner-ID: {partnerId}'\n    base_url: https://api.beamcheckout.com/api/v1/\n    managed_in: Bridge (Merchants > API Keys)\n  - name: PublishableKey\n    type: http\n    scheme: basic\n    usage: client-side requests to /client endpoints (e.g. card tokenization)\n    username: merchantId\n    password: publishable key\n    base_url: https://api.beamcheckout.com/client/v1/\n    note: publishable key is safe to be shared client-side\nenvironments:\n  - name: playground\n    base_url: https://playground.api.beamcheckout.com\n  - name: production\n    base_url: https://api.beamcheckout.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-checkout/refs/heads/main/authentication/beam-checkout-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Financial Services
- Payments
- Checkout
- Card Payments
- Webhooks
- Thailand
- Fintech
---
