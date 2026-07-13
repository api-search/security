---
api_key_in:
- header
api_specs:
- filename: basetrip-api-openapi.yml
  format: yaml
  label: Basetrip API
  slug: basetrip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/openapi/basetrip-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Basetrip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basetrip secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basetrip
provider_slug: basetrip
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/basetrip-api-openapi.yml
  type: apiKey
slug: basetrip-authentication
source_filename: basetrip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basetrip-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/basetrip-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/authentication/basetrip-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
---
