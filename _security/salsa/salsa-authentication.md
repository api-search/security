---
api_key_in: []
api_specs:
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Companies API
  slug: salsa-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Workers API
  slug: salsa-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Pay Schedules API
  slug: salsa-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payrolls API
  slug: salsa-payrolls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payments API
  slug: salsa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Onboarding & Sessions API
  slug: salsa-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Tax API
  slug: salsa-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Webhooks API
  slug: salsa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Salsa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salsa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Salsa
provider_slug: salsa
scheme_count: 1
schemes:
- description: 'Partner Bearer API key. Approved Salsa platform partners receive separate sandbox and production keys. Send as `Authorization: Bearer ${YOUR_API_TOKEN}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salsa-openapi.yml
  type: http
slug: salsa-authentication
source_filename: salsa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salsa-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Partner Bearer API key. Approved Salsa platform partners receive separate sandbox\n    and production keys. Send as `Authorization: Bearer ${YOUR_API_TOKEN}`.'\n  sources:\n  - openapi/salsa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/authentication/salsa-authentication.yml
summary_line: http · 1 scheme
tags:
- Payroll
- Embedded Finance
- Payroll as a Service
- Fintech
- Payments
- HR
- Tax
- Multi-Country
---
