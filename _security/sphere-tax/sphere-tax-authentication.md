---
api_key_in:
- header
api_specs:
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Tax Calculations API
  slug: sphere-tax-calculations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Transactions Export API
  slug: sphere-transactions-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Registrations and Filings API
  slug: sphere-registrations-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Nexus Monitoring API
  slug: sphere-nexus-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Exemptions API
  slug: sphere-exemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Webhooks API
  slug: sphere-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sphere Tax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sphere secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sphere
provider_slug: sphere-tax
scheme_count: 1
schemes:
- description: Sphere API key supplied in the X-API-KEY request header.
  in: header
  name: api_key
  parameter: X-API-KEY
  sources:
  - openapi/sphere-tax-openapi.yml
  type: apiKey
slug: sphere-tax-authentication
source_filename: sphere-tax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sphere-tax-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Sphere API key supplied in the X-API-KEY request header.\n  sources:\n  - openapi/sphere-tax-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/authentication/sphere-tax-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tax
- Sales Tax
- VAT
- GST
- Compliance
- FinTech
---
