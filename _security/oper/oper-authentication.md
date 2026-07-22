---
api_key_in: []
api_specs:
- filename: oper-api.json
  format: json
  label: Oper Connect API
  slug: oper-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-api.json
- filename: oper-resources.json
  format: json
  label: Oper Connect Resources API
  slug: oper-connect-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-resources.json
- filename: oper-metrics.json
  format: json
  label: Oper Connect Metrics API
  slug: oper-connect-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-metrics.json
- filename: oper-loan-request-webhook.json
  format: json
  label: Loan Request Webhook API
  slug: loan-request-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-loan-request-webhook.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oper secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oper
provider_slug: oper
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/oper-api.json
  - openapi/oper-metrics.json
  - openapi/oper-resources.json
  type: http
slug: oper-authentication
source_filename: oper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oper-api.json, openapi/oper-metrics.json, openapi/oper-resources.json\nsummary:\n  types:\n  - http\nschemes:\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/oper-api.json\n  - openapi/oper-metrics.json\n  - openapi/oper-resources.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/authentication/oper-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Vertical Software
- Fintech
- Mortgage
- Lending
- Loan Origination
- Digital Mortgage
- Underwriting
- Financial Services
---
