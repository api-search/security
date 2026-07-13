---
api_key_in:
- header
api_specs:
- filename: bindbee-api.yaml
  format: yaml
  label: Bindbee API
  slug: bindbee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bindbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bindbee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bindbee
provider_slug: bindbee
scheme_count: 1
schemes:
- description: Bearer API key in Authorization header. Also pass x-connector-token for the specific integration.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/bindbee-api.yaml
  type: apiKey
slug: bindbee-authentication
source_filename: bindbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bindbee-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer API key in Authorization header. Also pass x-connector-token for the specific\n    integration.\n  sources:\n  - openapi/bindbee-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/authentication/bindbee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ATS
- HR Integration
- HRIS
- Workforce
---
