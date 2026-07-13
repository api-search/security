---
api_key_in: []
api_specs:
- filename: candid-health-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: candid-health-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-openapi.yml
- filename: candid-health-openapi.yml
  format: yaml
  label: Candid Health Encounters API
  slug: candid-health-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Candid Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Candid Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Candid Health
provider_slug: candid-health
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication
  name: OAuthScheme
  scheme: bearer
  sources:
  - openapi/candid-health-openapi.yml
  type: http
slug: candid-health-authentication
source_filename: candid-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/candid-health-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuthScheme\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/candid-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/authentication/candid-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Medical Billing
- Revenue Cycle Management
- Healthcare
- Claims
- Eligibility
- Prior Authorization
- Remittance
- Patient Collections
- Credentialing
- Insurance
---
