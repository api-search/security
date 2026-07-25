---
api_key_in:
- header
api_specs:
- filename: roadsync-authenticated-api-openapi.yml
  format: yaml
  label: Roadsync authenticated API
  slug: roadsync-authenticated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-authenticated-api-openapi.yml
- filename: roadsync-brokers-api-openapi.yml
  format: yaml
  label: Roadsync brokers API
  slug: roadsync-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-brokers-api-openapi.yml
- filename: roadsync-department-api-openapi.yml
  format: yaml
  label: Roadsync department API
  slug: roadsync-department-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-department-api-openapi.yml
- filename: roadsync-directory-api-openapi.yml
  format: yaml
  label: Roadsync directory API
  slug: roadsync-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-directory-api-openapi.yml
- filename: roadsync-eta-api-openapi.yml
  format: yaml
  label: Roadsync eta API
  slug: roadsync-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-eta-api-openapi.yml
- filename: roadsync-funding-sources-api-openapi.yml
  format: yaml
  label: Roadsync funding sources API
  slug: roadsync-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-funding-sources-api-openapi.yml
- filename: roadsync-invoice-api-openapi.yml
  format: yaml
  label: Roadsync invoice API
  slug: roadsync-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-invoice-api-openapi.yml
- filename: roadsync-loads-api-openapi.yml
  format: yaml
  label: Roadsync loads API
  slug: roadsync-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-loads-api-openapi.yml
- filename: roadsync-location-api-openapi.yml
  format: yaml
  label: Roadsync location API
  slug: roadsync-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-location-api-openapi.yml
- filename: roadsync-payables-api-openapi.yml
  format: yaml
  label: Roadsync payables API
  slug: roadsync-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-payables-api-openapi.yml
- filename: roadsync-payees-api-openapi.yml
  format: yaml
  label: Roadsync payees API
  slug: roadsync-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-payees-api-openapi.yml
- filename: roadsync-payment-api-openapi.yml
  format: yaml
  label: Roadsync payment API
  slug: roadsync-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-payment-api-openapi.yml
- filename: roadsync-ping-api-openapi.yml
  format: yaml
  label: Roadsync ping API
  slug: roadsync-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-ping-api-openapi.yml
- filename: roadsync-product-api-openapi.yml
  format: yaml
  label: Roadsync product API
  slug: roadsync-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-product-api-openapi.yml
- filename: roadsync-shift-api-openapi.yml
  format: yaml
  label: Roadsync shift API
  slug: roadsync-shift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-shift-api-openapi.yml
- filename: roadsync-transactions-api-openapi.yml
  format: yaml
  label: Roadsync transactions API
  slug: roadsync-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-transactions-api-openapi.yml
- filename: roadsync-unauthenticated-api-openapi.yml
  format: yaml
  label: Roadsync unauthenticated API
  slug: roadsync-unauthenticated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-unauthenticated-api-openapi.yml
- filename: roadsync-workorders-api-openapi.yml
  format: yaml
  label: Roadsync workorders API
  slug: roadsync-workorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-workorders-api-openapi.yml
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
