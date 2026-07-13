---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Arcadia Plug API
  slug: arcadia-plug-api
  spec_type: OpenAPI
  url: https://api.arcadia.com/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arcadia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcadia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcadia
provider_slug: arcadia
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcadia-plug-openapi.yml
  type: http
slug: arcadia-authentication
source_filename: arcadia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcadia-plug-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/arcadia-plug-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/authentication/arcadia-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Clean Energy
- Billing Data
- Interval Data
- Carbon
- Solar
- Tariff
---
