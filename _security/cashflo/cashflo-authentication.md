---
api_key_in:
- header
api_specs:
- filename: cashflo-data-ingestion-openapi.json
  format: json
  label: CashFlo Data Ingestion API
  slug: cashflo-data-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashflo/refs/heads/main/openapi/cashflo-data-ingestion-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cashflo Authentication
name_suffix: Authentication
oauth_flows: []
overview: CashFlo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CashFlo
provider_slug: cashflo
scheme_count: 1
schemes:
- description: JWT authorization header
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/cashflo-data-ingestion-openapi.json
  type: apiKey
slug: cashflo-authentication
source_filename: cashflo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cashflo-data-ingestion-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT authorization header\n  sources:\n  - openapi/cashflo-data-ingestion-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashflo/refs/heads/main/authentication/cashflo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Accounts Payable
- Payments
- Working Capital
- Supply Chain Finance
- ERP Integration
- Compliance
- India
---
