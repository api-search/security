---
api_key_in: []
api_specs:
- filename: ukg-pro-hcm-openapi.yml
  format: yaml
  label: UKG Pro HCM API
  slug: ukg-pro-hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/openapi/ukg-pro-hcm-openapi.yml
- filename: ukg-pro-wfm-openapi.yml
  format: yaml
  label: UKG Pro Workforce Management API
  slug: ukg-pro-wfm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/openapi/ukg-pro-wfm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ukg Authentication
name_suffix: Authentication
oauth_flows: []
overview: UKG secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UKG
provider_slug: ukg
scheme_count: 2
schemes:
- description: Basic authentication with service account credentials plus US-API-Key header
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ukg-pro-hcm-openapi.yml
  type: http
- description: OAuth 2.0 bearer token with WFM API key header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ukg-pro-wfm-openapi.yml
  type: http
slug: ukg-authentication
source_filename: ukg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ukg-pro-hcm-openapi.yml, openapi/ukg-pro-wfm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with service account credentials plus US-API-Key header\n  sources:\n  - openapi/ukg-pro-hcm-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token with WFM API key header\n  sources:\n  - openapi/ukg-pro-wfm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/authentication/ukg-authentication.yml
summary_line: http · 2 schemes
tags:
- Human Capital Management
- HCM
- Workforce Management
- HR
- Payroll
- Time and Attendance
- Benefits
- Scheduling
---
