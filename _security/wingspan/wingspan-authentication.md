---
api_key_in: []
api_specs:
- filename: wingspan-payments-openapi-original.yml
  format: yaml
  label: Wingspan Payments API
  slug: wingspan-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-payments-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wingspan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wingspan secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wingspan
provider_slug: wingspan
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wingspan-payments-openapi-original.yml
  type: http
slug: wingspan-authentication
source_filename: wingspan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wingspan-payments-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wingspan-payments-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/authentication/wingspan-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Payroll
- Contractors
- Invoicing
- Taxes
- Fintech
- Freelance Economy
---
