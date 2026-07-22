---
api_key_in:
- header
auth_types:
- apiKey
description: Tiptop authenticates with API keys. Each partner account gets four keys — a public and private key pair for both the test (sandbox) and live environments. Public keys identify the account client-side (tiptop.js, mobile) and are used to generate tokens; private (server) keys are sent on server-to-server Order Management API calls in the api-key request header. Objects created in one mode cannot be manipulated by the other.
kind: authentication
layout: security
method: searched
name: Tiptop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tiptop secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tiptop
provider_slug: tiptop
scheme_count: 2
schemes:
- audience: server
  description: 'Private/server API key sent as the api-key header on Order Management API requests (capture, void, refund). Provided via secure email or the merchant dashboard. Requests are JSON (Content-Type: application/json).'
  in: header
  name: api-key
  parameter: api-key
  sources:
  - https://docs.tiptop.com/direct/order-management-apis/capture/
  - https://github.com/tiptopxyz/magento/blob/master/Gateway/Http/TransferFactory.php
  type: apiKey
- audience: browser
  description: Public API key set in the _tiptop_config object when loading tiptop.js; safely shareable, used to initialize the checkout/messaging library and generate tokens for further authentication.
  in: client-config
  name: public_api_key
  parameter: public_api_key
  sources:
  - https://docs.tiptop.com/direct/tiptop-js-reference/overview/
  - https://docs.tiptop.com/api-keys/
  type: apiKey
slug: tiptop-authentication
source_filename: tiptop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.tiptop.com/api-keys/\nsource: >-\n  https://docs.tiptop.com/api-keys/ plus the first-party Magento gateway source\n  (https://github.com/tiptopxyz/magento — Gateway/Http/TransferFactory.php sets\n  the api-key request header). Tiptop publishes no OpenAPI, so this profile is\n  captured from docs and first-party integration code rather than derived from\n  a spec.\ndescription: >-\n  Tiptop authenticates with API keys. Each partner account gets four keys — a\n  public and private key pair for both the test (sandbox) and live\n  environments. Public keys identify the account client-side (tiptop.js,\n  mobile) and are used to generate tokens; private (server) keys are sent on\n  server-to-server Order Management API calls in the api-key request header.\n  Objects created in one mode cannot be manipulated by the other.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: api-key\n\
  \    type: apiKey\n    in: header\n    parameter: api-key\n    audience: server\n    description: >-\n      Private/server API key sent as the api-key header on Order Management API\n      requests (capture, void, refund). Provided via secure email or the\n      merchant dashboard. Requests are JSON (Content-Type: application/json).\n    sources:\n      - https://docs.tiptop.com/direct/order-management-apis/capture/\n      - https://github.com/tiptopxyz/magento/blob/master/Gateway/Http/TransferFactory.php\n  - name: public_api_key\n    type: apiKey\n    in: client-config\n    parameter: public_api_key\n    audience: browser\n    description: >-\n      Public API key set in the _tiptop_config object when loading tiptop.js;\n      safely shareable, used to initialize the checkout/messaging library and\n      generate tokens for further authentication.\n    sources:\n      - https://docs.tiptop.com/direct/tiptop-js-reference/overview/\n      - https://docs.tiptop.com/api-keys/\nenvironments:\n\
  \  - {name: test, notes: Sandbox mode; test key pair; staging hosts api-stage.tiptop.com and cdn-stage.tiptop.com.}\n  - {name: live, notes: Production key pair issued after a completed test order during partner onboarding.}\nkey_retrieval: Merchant Portal (https://tiptop.com/partner/auth — as of 2026-07-21 this redirects to https://mother.ai/)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiptop/refs/heads/main/authentication/tiptop-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- FinTech
- Trade-In
- Checkout
- Commerce
- Pay Over Time
---
