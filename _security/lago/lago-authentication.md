---
api_key_in: []
api_specs:
- filename: lago-openapi.yml
  format: yaml
  label: Lago API
  slug: lago-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lago secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lago
provider_slug: lago
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lago-openapi.yml
  type: http
slug: lago-authentication
source_filename: lago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lago-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lago-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/authentication/lago-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Metering
- Open Source
- Usage-Based
---
