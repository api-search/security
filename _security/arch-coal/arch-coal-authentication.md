---
api_key_in:
- header
api_specs:
- filename: arch-coal-investor-relations-api.yaml
  format: yaml
  label: Arch Coal Investor Relations
  slug: arch-coal-investor-relations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/openapi/arch-coal-investor-relations-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arch Coal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arch Coal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arch Coal
provider_slug: arch-coal
scheme_count: 1
schemes:
- description: API key for Arch Coal investor data access
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/arch-coal-investor-relations-api.yaml
  type: apiKey
slug: arch-coal-authentication
source_filename: arch-coal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arch-coal-investor-relations-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for Arch Coal investor data access\n  sources:\n  - openapi/arch-coal-investor-relations-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/authentication/arch-coal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
---
