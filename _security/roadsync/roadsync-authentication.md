---
api_key_in:
- header
api_specs:
- filename: roadsync-rspay-openapi.json
  format: json
  label: RoadSyncPay Public API
  slug: roadsyncpay-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-rspay-openapi.json
- filename: roadsync-invoice-openapi.json
  format: json
  label: Invoice API
  slug: invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-invoice-openapi.json
- filename: roadsync-company-openapi.json
  format: json
  label: Company API
  slug: company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-company-openapi.json
- filename: roadsync-workorder-openapi.json
  format: json
  label: WorkOrders API
  slug: workorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-workorder-openapi.json
- filename: roadsync-payment-openapi.json
  format: json
  label: Payment API
  slug: payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-payment-openapi.json
- filename: roadsync-client-api-openapi.json
  format: json
  label: Legacy Client API
  slug: legacy-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-client-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Roadsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roadsync secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Roadsync
provider_slug: roadsync
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/roadsync-client-api-openapi.json
  - openapi/roadsync-company-openapi.json
  - openapi/roadsync-invoice-openapi.json
  - openapi/roadsync-payment-openapi.json
  - openapi/roadsync-rspay-openapi.json
  - openapi/roadsync-workorder-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: session_token
  scheme: bearer
  sources:
  - openapi/roadsync-client-api-openapi.json
  type: http
slug: roadsync-authentication
source_filename: roadsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/roadsync-client-api-openapi.json, openapi/roadsync-company-openapi.json, openapi/roadsync-invoice-openapi.json,\n  openapi/roadsync-payment-openapi.json, openapi/roadsync-rspay-openapi.json, openapi/roadsync-workorder-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/roadsync-client-api-openapi.json\n  - openapi/roadsync-company-openapi.json\n  - openapi/roadsync-invoice-openapi.json\n  - openapi/roadsync-payment-openapi.json\n  - openapi/roadsync-rspay-openapi.json\n  - openapi/roadsync-workorder-openapi.json\n- name: session_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/roadsync-client-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/authentication/roadsync-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Financial Services
- Payments
- Logistics
- Trucking
- Invoicing
- Transportation
- Fintech
---
