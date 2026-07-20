---
api_key_in:
- header
- body
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aplazo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aplazo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aplazo
provider_slug: aplazo
scheme_count: 2
schemes:
- description: Per-request merchant credential headers sent on every call to the Aplazo merchant API.
  in: header
  name: merchantCredentialHeaders
  parameter_names:
  - merchant_id
  - api_token
  sources:
  - github.com/aplazo/php.aplazo-magento-2-payment-gateway Service/ApiService.php
  type: apiKey
- bearer_format: JWT
  description: JWT bearer token returned in the Authorization field of POST /api/auth, passed as the Authorization header on loan-origination requests.
  name: bearerAuth
  obtained_via:
    operation: POST /api/auth
    request_body: '{ "apiToken": "...", "merchantId": "..." }'
    returns: Authorization (JWT)
  scheme: bearer
  sources:
  - github.com/aplazo/php.aplazo-magento-2-payment-gateway Service/ApiService.php
  type: http
slug: aplazo-authentication
source_filename: aplazo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/aplazo/php.aplazo-magento-2-payment-gateway (Service/ApiService.php)\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, body]\n  token_format: jwt\n  description: >-\n    Aplazo's merchant API uses a two-part credential (apiToken + merchantId)\n    issued in the merchant's Aplazo account. Every request carries the\n    credential as the merchant_id and api_token headers. Loan origination first\n    exchanges the credential at POST /api/auth for a short-lived JWT which is\n    then sent as an Authorization bearer token on subsequent calls.\nschemes:\n  - name: merchantCredentialHeaders\n    type: apiKey\n    in: header\n    parameter_names: [merchant_id, api_token]\n    description: >-\n      Per-request merchant credential headers sent on every call to the Aplazo\n      merchant API.\n    sources:\n      - github.com/aplazo/php.aplazo-magento-2-payment-gateway Service/ApiService.php\n  - name: bearerAuth\n\
  \    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      JWT bearer token returned in the Authorization field of POST /api/auth,\n      passed as the Authorization header on loan-origination requests.\n    obtained_via:\n      operation: POST /api/auth\n      request_body: '{ \"apiToken\": \"...\", \"merchantId\": \"...\" }'\n      returns: Authorization (JWT)\n    sources:\n      - github.com/aplazo/php.aplazo-magento-2-payment-gateway Service/ApiService.php\ncredentials:\n  issued_in: Aplazo merchant account\n  fields: [apiToken, merchantId]\ndocs: https://github.com/aplazo/php.aplazo-magento-2-payment-gateway\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aplazo/refs/heads/main/authentication/aplazo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- BNPL
- Buy Now Pay Later
- Installments
- Fintech
- Lending
- Mexico
- Checkout
- E-commerce
---
