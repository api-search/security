---
api_key_in: []
api_specs:
- filename: ukg-pro-benefits-api-openapi.yml
  format: yaml
  label: UKG Pro Benefits API
  slug: ukg-pro-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/openapi/ukg-pro-benefits-api-openapi.yml
- filename: ukg-pro-employment-api-openapi.yml
  format: yaml
  label: UKG Pro Employment API
  slug: ukg-pro-employment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/openapi/ukg-pro-employment-api-openapi.yml
- filename: ukg-pro-pay-api-openapi.yml
  format: yaml
  label: UKG Pro Pay API
  slug: ukg-pro-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/openapi/ukg-pro-pay-api-openapi.yml
- filename: ukg-pro-people-api-openapi.yml
  format: yaml
  label: UKG Pro People API
  slug: ukg-pro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/openapi/ukg-pro-people-api-openapi.yml
- filename: ukg-pro-recruiting-api-openapi.yml
  format: yaml
  label: UKG Pro Recruiting API
  slug: ukg-pro-recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/openapi/ukg-pro-recruiting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ukg Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: UKG Pro secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UKG Pro
provider_slug: ukg-pro
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using a UKG Pro web service account.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ukg-pro-openapi.yml
  type: http
- bearerFormat: JWT
  description: Bearer Authorization Token issued for onboarding and recruiting APIs.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ukg-pro-openapi.yml
  type: http
slug: ukg-pro-authentication
source_filename: ukg-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ukg-pro-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using a UKG Pro web service account.\n  sources:\n  - openapi/ukg-pro-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer Authorization Token issued for onboarding and recruiting APIs.\n  sources:\n  - openapi/ukg-pro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukg-pro/refs/heads/main/authentication/ukg-pro-authentication.yml
summary_line: http · 2 schemes
tags:
- HCM
- HR
- Payroll
- Benefits Administration
- Talent Management
- Workforce Management
- HRIS
---
