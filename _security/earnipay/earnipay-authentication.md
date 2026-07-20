---
api_key_in:
- header
api_specs:
- filename: earnipay-e-invoicing-openapi-original.json
  format: json
  label: Earnipay Invoicing API
  slug: earnipay-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-e-invoicing-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Earnipay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Earnipay secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Earnipay
provider_slug: earnipay
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Enter JWT token
  name: JWT-auth
  scheme: bearer
  sources:
  - openapi/earnipay-e-invoicing-openapi-original.json
  type: http
- description: API Key for third-party integrations
  in: header
  name: API-Key
  parameter: X-API-Key
  sources:
  - openapi/earnipay-e-invoicing-openapi-original.json
  type: apiKey
slug: earnipay-authentication
source_filename: earnipay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/earnipay-e-invoicing-openapi-original.json\ndocs: https://docs.earnipay.com/docs/authentication\nnotes: >-\n  User-facing flows authenticate with a JWT bearer token obtained from\n  POST /v1/auth/login (register via POST /v1/auth/signup, verify with\n  POST /v1/auth/verify-email). Access tokens are refreshed via\n  POST /v1/auth/refresh and invalidated via POST /v1/auth/logout. Send the JWT\n  in the Authorization header as `Bearer <token>`. Third-party/server-to-server\n  integrations use a static API key sent in the `X-API-Key` header. No OAuth 2.0\n  authorization-server or scope surface is exposed.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: JWT-auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter JWT token\n  sources:\n  - openapi/earnipay-e-invoicing-openapi-original.json\n- name: API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n\
  \  description: API Key for third-party integrations\n  sources:\n  - openapi/earnipay-e-invoicing-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/authentication/earnipay-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- E-Invoicing
- Invoicing
- FIRS
- NRS
- Tax
- Compliance
- Fintech
- Nigeria
- Payments
- Financial Services
---
