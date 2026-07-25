---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ozonru Authentication
name_suffix: Authentication
oauth_flows: []
overview: OZON.ru declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OZON.ru
provider_slug: ozonru
scheme_count: 1
schemes:
- id: ozon_seller_headers
  in: header
  required_headers:
  - description: Numeric seller/client identifier. A non-integer value is rejected with HTTP 400 {"code":3,"message":"Client-Id header value should be positive integer"} (verified live).
    format: positive integer
    name: Client-Id
  - description: Secret API key issued in the seller cabinet. An invalid key is rejected with HTTP 404 {"code":5,"message":"Invalid Api-Key, please check the key and try again"} (verified live).
    format: UUID/secret string
    name: Api-Key
  transport: https-only (TLS 1.3)
  type: apiKey
slug: ozonru-authentication
source_filename: ozonru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  live probe of https://api-seller.ozon.ru + OZON Seller API docs\n  (https://docs.ozon.ru/api/seller/)\napi: OZON Seller API\nbase_url: https://api-seller.ozon.ru\nsummary: >-\n  The OZON Seller API authenticates every request with two required HTTP\n  headers: a numeric Client-Id and a secret Api-Key, both issued in the seller\n  dashboard (API keys section). There is no OAuth flow. Requests are made over\n  HTTPS/TLS 1.3.\nschemes:\n- id: ozon_seller_headers\n  type: apiKey\n  in: header\n  required_headers:\n  - name: Client-Id\n    format: positive integer\n    description: >-\n      Numeric seller/client identifier. A non-integer value is rejected with\n      HTTP 400 {\"code\":3,\"message\":\"Client-Id header value should be positive\n      integer\"} (verified live).\n  - name: Api-Key\n    format: UUID/secret string\n    description: >-\n      Secret API key issued in the seller cabinet. An invalid key is rejected\n\
  \      with HTTP 404 {\"code\":5,\"message\":\"Invalid Api-Key, please check the key\n      and try again\"} (verified live).\n  transport: https-only (TLS 1.3)\nevidence:\n- kind: live-probe\n  detail: >-\n    POST https://api-seller.ozon.ru/v1/warehouse/list with malformed Client-Id\n    returned HTTP 400 code 3; with a valid-format but wrong Api-Key returned\n    HTTP 404 code 5.\nnotes: >-\n  API keys are provisioned per seller in the OZON Seller cabinet and can be\n  scoped by role (Admin / read-only / etc.) in the seller UI; there is no\n  standards-based OAuth2/OIDC scopes model, so no scopes/ artifact is derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozonru/refs/heads/main/authentication/ozonru-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Retail
- E-Commerce
- Marketplace
- Seller API
- Russia
- Logistics
---
