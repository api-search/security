---
api_key_in: []
api_specs:
- filename: humana-openapi.yml
  format: yaml
  label: Humana FHIR Clinical Data API
  slug: humana-fhir-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humana/refs/heads/main/openapi/humana-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Humana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Humana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Humana
provider_slug: humana
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/humana-openapi.yml
  type: http
slug: humana-authentication
source_filename: humana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/humana-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/humana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humana/refs/heads/main/authentication/humana-authentication.yml
summary_line: http · 1 scheme
tags:
- FHIR
- Health Insurance
- Healthcare
- Interoperability
- Medicare
- Fortune 100
---
