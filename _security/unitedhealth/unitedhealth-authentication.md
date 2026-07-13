---
api_key_in: []
api_specs:
- filename: unitedhealth-optum-api-openapi.yml
  format: yaml
  label: UnitedHealth Group Optum API
  slug: optum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealth/refs/heads/main/openapi/unitedhealth-optum-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unitedhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: UnitedHealth Group secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UnitedHealth Group
provider_slug: unitedhealth
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained via authorization code flow
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unitedhealth-optum-api-openapi.yml
  type: http
slug: unitedhealth-authentication
source_filename: unitedhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unitedhealth-optum-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained via authorization code flow\n  sources:\n  - openapi/unitedhealth-optum-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitedhealth/refs/heads/main/authentication/unitedhealth-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Health Insurance
- FHIR
- Claims
- Interoperability
- Fortune 100
---
