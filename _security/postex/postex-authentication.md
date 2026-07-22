---
api_key_in:
- header
api_specs:
- filename: postex-order-openapi.yml
  format: yaml
  label: PostEx Merchant Order Integration API
  slug: postex-merchant-order-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postex/refs/heads/main/openapi/postex-order-openapi.yml
auth_types:
- apiKey
description: PostEx's merchant Order Integration API authenticates every request with a merchant API token issued from the PostEx merchant dashboard, supplied in the `token` request header. No OAuth or OpenID Connect surface was found.
kind: authentication
layout: security
method: searched
name: Postex Authentication
name_suffix: Authentication
oauth_flows: []
overview: PostEx secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PostEx
provider_slug: postex
scheme_count: 1
schemes:
- description: Merchant API token issued from the PostEx merchant dashboard, sent in the `token` request header on every Order Integration API call.
  in: header
  name: merchantToken
  parameter_name: token
  sources:
  - openapi/postex-order-openapi.yml
  type: apiKey
slug: postex-authentication
source_filename: postex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  Live probe of https://api.postex.pk merchant Order Integration API. Every\n  endpoint returns HTTP 400 \"Missing request header 'token'\" when called\n  without credentials, confirming an apiKey-in-header auth model. The CORS\n  Access-Control-Allow-Headers on the host also advertise: X-Api-Key,\n  authorization, skip, token, X-Device-Id, X-LANG.\ndescription: >-\n  PostEx's merchant Order Integration API authenticates every request with a\n  merchant API token issued from the PostEx merchant dashboard, supplied in the\n  `token` request header. No OAuth or OpenID Connect surface was found.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\nschemes:\n  - name: merchantToken\n    type: apiKey\n    in: header\n    parameter_name: token\n    description: >-\n      Merchant API token issued from the PostEx merchant dashboard, sent in the\n      `token` request header on every Order Integration\
  \ API call.\n    sources:\n      - openapi/postex-order-openapi.yml\nnotes: >-\n  The host's CORS policy additionally allows the headers X-Api-Key,\n  authorization, and skip, but only the `token` header is required and enforced\n  by the Order Integration API endpoints probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postex/refs/heads/main/authentication/postex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Courier
- Shipping
- E-commerce
- Fulfillment
- Cash on Delivery
- Payments
- Fintech
- Pakistan
---
