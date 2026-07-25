---
api_key_in: []
api_specs:
- filename: gett-authentication-api-openapi.yml
  format: yaml
  label: Gett Authentication API
  slug: gett-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-authentication-api-openapi.yml
- filename: gett-employee-management-api-openapi.yml
  format: yaml
  label: Gett Employee Management API
  slug: gett-employee-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-employee-management-api-openapi.yml
- filename: gett-finance-api-openapi.yml
  format: yaml
  label: Gett Finance API
  slug: gett-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-finance-api-openapi.yml
- filename: gett-orders-api-openapi.yml
  format: yaml
  label: Gett Orders API
  slug: gett-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-orders-api-openapi.yml
- filename: gett-products-api-openapi.yml
  format: yaml
  label: Gett Products API
  slug: gett-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-products-api-openapi.yml
- filename: gett-webhooks-api-openapi.yml
  format: yaml
  label: Gett Webhooks API
  slug: gett-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/gett-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gett Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gett secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gett
provider_slug: gett
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from /oauth/token endpoint. Valid for 899 seconds.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: gett-authentication
source_filename: gett-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from /oauth/token endpoint. Valid for 899 seconds.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/authentication/gett-authentication.yml
summary_line: http · 1 scheme
tags:
- Ground Transportation
- Corporate Travel
- Ride Booking
- Business Travel
- Expense Management
---
