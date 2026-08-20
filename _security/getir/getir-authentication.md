---
api_key_in:
- header
api_specs:
- filename: getir-food-openapi.yml
  format: yaml
  label: GetirFood API
  slug: getirfood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-food-openapi.yml
auth_types:
- custom-token
description: 'GetirFood does not declare securityDefinitions in its Swagger 2.0 document. Authentication is a two-step, documented-only model: POST /auth/login exchanges the company/restaurant secret keys for a bearer-style opaque token, which is then supplied as a REQUIRED `token` request HEADER on every other operation (57 of 62 operations carry it as an explicit header parameter). There is no OAuth 2.0, no OpenID Connect and no scope surface, so scopes/ is intentionally absent for this provider.'
kind: authentication
layout: security
method: searched
name: Getir Authentication
name_suffix: Authentication
oauth_flows: []
overview: Getir secures its APIs with custom-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Getir
provider_slug: getir
scheme_count: 1
schemes:
- applies_to_operations: 57
  description: Opaque session token returned by POST /auth/login. Sent on every authenticated request as the `token` HTTP header. The Swagger document models it as an individual header parameter on each operation rather than as a global security scheme.
  in: header
  name: token
  parameter: token
  required: true
  sources:
  - openapi/getir-food-openapi.yml
  - https://developers.getir.com/food/documentation/giris
  type: apiKey
slug: getir-authentication
source_filename: getir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://developers.getir.com/food/documentation/giris — \"Authentication\" section, served by\n  https://food-pos-api-gateway.getirapi.com/v1/documentations/contents?title=4&language=en\ndocs: https://developers.getir.com/food/documentation/giris\ndescription: >-\n  GetirFood does not declare securityDefinitions in its Swagger 2.0 document. Authentication is\n  a two-step, documented-only model: POST /auth/login exchanges the company/restaurant secret\n  keys for a bearer-style opaque token, which is then supplied as a REQUIRED `token` request\n  HEADER on every other operation (57 of 62 operations carry it as an explicit header\n  parameter). There is no OAuth 2.0, no OpenID Connect and no scope surface, so scopes/ is\n  intentionally absent for this provider.\nsummary:\n  types: [custom-token]\n  api_key_in: [header]\n  oauth2_flows: []\n  declared_in_spec: false\n  documented_in_docs: true\nschemes:\n- name: token\n  type:\
  \ apiKey\n  in: header\n  parameter: token\n  required: true\n  applies_to_operations: 57\n  description: >-\n    Opaque session token returned by POST /auth/login. Sent on every authenticated request as\n    the `token` HTTP header. The Swagger document models it as an individual header parameter\n    on each operation rather than as a global security scheme.\n  sources:\n  - openapi/getir-food-openapi.yml\n  - https://developers.getir.com/food/documentation/giris\nlogin:\n  operation_id: postAuthLogin\n  method: POST\n  path: /auth/login\n  request_schema: '#/definitions/Login Schema'\n  response_schema: '#/definitions/Login Response Schema'\n  credentials:\n  - name: appSecretKey\n    description: Secret key issued to the integrating company (POS / integrator).\n  - name: restaurantSecretKey\n    description: Secret key issued per restaurant being managed.\n  spec_description: >-\n    \"Authentication is performed via HTTP Basic Auth. Use your appSecretKey and\n    restaurantSecretKey\
  \ taking new token for reaching all routes.\" (verbatim from the\n    operation description in the Swagger document)\n  note: >-\n    The operation description says \"HTTP Basic Auth\" while the request is modelled as a JSON\n    body carrying the two secret keys; the docs describe it as a secret-key login. Recorded as\n    published — not reconciled by us.\ntoken:\n  ttl: 3600\n  ttl_human: 1 hour\n  refresh: Call POST /auth/login again to obtain a new token; there is no refresh-token flow.\n  docs_quote: >-\n    \"The validity period of the token is 1 hour. As the token will expire at the end of this\n    period, you need to login again and get a new one.\"\ncredential_issuance:\n  process: >-\n    Credentials are not self-service. A restaurant asks its POS/integrator company to request\n    an account from Getir; both test and live credentials are issued by Getir.\n  contact: getiryemekapi@getir.com\n  docs: https://developers.getir.com/food/documentation/giris\nwebhook_authentication:\n\
  \  mechanism: x-api-key\n  direction: Getir -> partner (outbound order push)\n  description: >-\n    Partners register a new-order URL and a cancel-order URL plus a single `x-api-key` value\n    that Getir sends on both callbacks. The same x-api-key value must be used for both URLs.\n  detail: asyncapi/getir-food-webhooks.yml\ntransport_security:\n  tls_minimum: TLSv1.2_2019\n  docs_quote: 'TLS Versiyon: TLSv1.2_2019 and above'\n  source: https://developers.getir.com/food/documentation/giris\nx-evidence:\n  fetched: '2026-07-31'\n  spec: https://food-external-api-gateway.getirapi.com/swagger.json\n  docs_api: https://food-pos-api-gateway.getirapi.com/v1/documentations/contents?title=4&language=en\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/authentication/getir-authentication.yml
summary_line: custom-token · 1 scheme
tags:
- Company
- Food Delivery
- Grocery Delivery
- On-Demand Delivery
- Logistics
- Restaurant
- Point-of-Sale
- Marketplace
- Turkey
- Partner Integration
---
