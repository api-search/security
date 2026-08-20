---
api_key_in:
- header
api_specs:
- filename: scalapay-instore-api-openapi.yml
  format: yaml
  label: Scalapay Instore API
  slug: scalapay-instore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-instore-api-openapi.yml
- filename: scalapay-orders-api-openapi.yml
  format: yaml
  label: Scalapay Orders API
  slug: scalapay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-orders-api-openapi.yml
- filename: scalapay-reporting-api-openapi.yml
  format: yaml
  label: Scalapay Reporting API
  slug: scalapay-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-reporting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Scalapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalapay secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scalapay
provider_slug: scalapay
scheme_count: 2
schemes:
- applies_to: default security for all operations (online orders, payments, reporting)
  description: API key authentication using the Authorization header with a Bearer token.
  format: Bearer <secret_api_key>
  in: header
  key_prefix: sp_
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/scalapay-openapi-original.yml
  type: apiKey
- applies_to:
  - POST /v1/instore/orders
  - GET /v1/instore/orders/{token}
  - GET /v1/instore/orders/references
  - POST /v1/instore/orders/{token}/refund
  - POST /v2/instore/paybylink/orders
  - POST /v2/instore/paybylink/orders/{token}/void
  description: API key authentication for instore endpoints using the Authorization header with a Bearer token.
  format: Bearer <device_api_key>
  in: header
  name: InstoreApiKeyAuth
  note: Declared in components.securitySchemes alongside ApiKeyAuth. The pay-by-link operations explicitly require the device bearer token, not the merchant token. The mechanical derive pass only surfaced ApiKeyAuth because it is the sole scheme in the document-level security[] block; this scheme was added from the specification's components and the in-store reference pages.
  parameter: Authorization
  sources:
  - openapi/scalapay-openapi-original.yml
  type: apiKey
slug: scalapay-authentication
source_filename: scalapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/scalapay-openapi-original.yml\ndocs: https://developers.scalapay.com/reference/api-architecture\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: static bearer API key, environment-scoped, with a second device-scoped key for in-store\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <secret_api_key>'\n  description: API key authentication using the Authorization header with a Bearer token.\n  applies_to: default security for all operations (online orders, payments, reporting)\n  key_prefix: sp_\n  sources:\n  - openapi/scalapay-openapi-original.yml\n- name: InstoreApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <device_api_key>'\n  description: API key authentication for instore endpoints using the Authorization header with a Bearer token.\n  applies_to:\n  - POST /v1/instore/orders\n\
  \  - GET /v1/instore/orders/{token}\n  - GET /v1/instore/orders/references\n  - POST /v1/instore/orders/{token}/refund\n  - POST /v2/instore/paybylink/orders\n  - POST /v2/instore/paybylink/orders/{token}/void\n  note: >-\n    Declared in components.securitySchemes alongside ApiKeyAuth. The pay-by-link operations explicitly\n    require the device bearer token, not the merchant token. The mechanical derive pass only surfaced\n    ApiKeyAuth because it is the sole scheme in the document-level security[] block; this scheme was\n    added from the specification's components and the in-store reference pages.\n  sources:\n  - openapi/scalapay-openapi-original.yml\nkey_management:\n  issuer: Scalapay Merchant Portal (Developer section)\n  portal: https://partner.scalapay.com/login\n  environment_scoped: true\n  environments:\n    - {name: sandbox, base_url: 'https://integration.api.scalapay.com'}\n    - {name: production, base_url: 'https://api.scalapay.com'}\n  rotation_policy: not published\n\
  \  expiry: not published\n  scopes: none — the key is unscoped; there is no OAuth or permission model\nfailure:\n  status: 401\n  body: '\"Unauthorized\"'\n  note: >-\n    The 401 body is a bare JSON string, not the {errorCode, errorId, message, httpStatusCode} envelope\n    used by other errors. Documented causes are a missing \"Bearer \" prefix, more than one space after\n    \"Bearer\", or using the wrong environment's key.\ntransport_security:\n  tls_minimum: TLS 1.2\n  observed: TLSv1.3 on api.scalapay.com and integration.api.scalapay.com\n  hsts: true\n  hsts_max_age: 63072000\n  artifact: security/scalapay-domain-security.yml\noidc: false\noauth2: false\nmtls: false\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n    - https://developers.scalapay.com/reference/api-architecture\n    - https://developers.scalapay.com/reference/post_v1-instore-orders\n    - https://developers.scalapay.com/reference/post_v2-instore-paybylink-orders\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/authentication/scalapay-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- Buy Now Pay Later
- BNPL
- Instalments
- E-Commerce
- Checkout
- Financial-Services
- Point-of-Sale
- Reconciliation
- Europe
- Company
---
