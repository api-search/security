---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Easypay Authentication
name_suffix: Authentication
oauth_flows: []
overview: EasyPay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EasyPay
provider_slug: easypay
scheme_count: 1
schemes:
- description: 'Fawaterak/EasyPay authenticates every API call with a vendor API token issued from the merchant dashboard, sent in the HTTP Authorization header as "Authorization: Bearer <token>". A missing token returns {"status":"error","message":{"token":["Token Is Missing"]}}; an invalid token returns {"token":["Invalid Token or inactive vendor."]}.'
  format: Bearer <vendor-token>
  header_name: Authorization
  in: header
  name: vendorToken
  scheme: bearer
  sources:
  - live-probe:https://app.fawaterk.com/api/v2/invoiceInitPay
  type: http
slug: easypay-authentication
source_filename: easypay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  Live probe of https://app.fawaterk.com/api/v2/ (Authorization: Bearer challenge)\n  and https://app.fawaterk.com/documentation\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: vendorToken\n  type: http\n  scheme: bearer\n  description: >-\n    Fawaterak/EasyPay authenticates every API call with a vendor API token issued\n    from the merchant dashboard, sent in the HTTP Authorization header as\n    \"Authorization: Bearer <token>\". A missing token returns\n    {\"status\":\"error\",\"message\":{\"token\":[\"Token Is Missing\"]}}; an invalid token\n    returns {\"token\":[\"Invalid Token or inactive vendor.\"]}.\n  in: header\n  header_name: Authorization\n  format: Bearer <vendor-token>\n  sources:\n  - live-probe:https://app.fawaterk.com/api/v2/invoiceInitPay\nnotes: >-\n  No OpenAPI/Swagger spec is published (both /openapi.json and /swagger.json return\n\
  \  the SPA HTML shell). The scheme above was confirmed by live probing the production\n  API host: sending \"Authorization: Bearer [example key]\" changes the error from \"Token Is\n  Missing\" to \"Invalid Token or inactive vendor.\", confirming a header-carried bearer\n  vendor token. No OAuth2/OIDC surface was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easypay/refs/heads/main/authentication/easypay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Payment Gateway
- Invoicing
- Fintech
- E-commerce
- Egypt
- Online Payments
---
