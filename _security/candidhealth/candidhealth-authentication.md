---
api_key_in: []
api_specs:
- filename: candidhealth-auth-api-openapi.yml
  format: yaml
  label: Candid Health Auth API
  slug: candidhealth-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-auth-api-openapi.yml
- filename: candidhealth-charge-capture-api-openapi.yml
  format: yaml
  label: Candid Health Charge Capture API
  slug: candidhealth-charge-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-charge-capture-api-openapi.yml
- filename: candidhealth-eligibility-api-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: candidhealth-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-eligibility-api-openapi.yml
- filename: candidhealth-encounters-api-openapi.yml
  format: yaml
  label: Candid Health Encounters API
  slug: candidhealth-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-encounters-api-openapi.yml
- filename: candidhealth-events-api-openapi.yml
  format: yaml
  label: Candid Health Events API
  slug: candidhealth-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-events-api-openapi.yml
- filename: candidhealth-fee-schedules-api-openapi.yml
  format: yaml
  label: Candid Health Fee Schedules API
  slug: candidhealth-fee-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-fee-schedules-api-openapi.yml
- filename: candidhealth-insurance-adjudications-api-openapi.yml
  format: yaml
  label: Candid Health Insurance Adjudications API
  slug: candidhealth-insurance-adjudications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-insurance-adjudications-api-openapi.yml
- filename: candidhealth-payers-api-openapi.yml
  format: yaml
  label: Candid Health Payers API
  slug: candidhealth-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-payers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Candidhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Candid Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Candid Health
provider_slug: candidhealth
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth bearer token obtained from POST /auth/v2/token. Send as `Authorization: Bearer <access_token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/candidhealth-openapi.yml
  type: http
slug: candidhealth-authentication
source_filename: candidhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/candidhealth-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth bearer token obtained from POST /auth/v2/token. Send as `Authorization:\n    Bearer <access_token>`.'\n  sources:\n  - openapi/candidhealth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/authentication/candidhealth-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Medical Billing
- Revenue Cycle
- Claims
- Eligibility
---
