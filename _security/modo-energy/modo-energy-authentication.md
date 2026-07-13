---
api_key_in:
- header
api_specs:
- filename: modo-energy-openapi.yml
  format: yaml
  label: Modo Energy
  slug: modo-energy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modo-energy/refs/heads/main/openapi/modo-energy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Modo Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modo Energy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Modo Energy
provider_slug: modo-energy
scheme_count: 1
schemes:
- description: Public API token obtained from your Modo Energy account.
  in: header
  name: apiKey
  parameter: X-Token
  sources:
  - openapi/modo-energy-openapi.yml
  type: apiKey
slug: modo-energy-authentication
source_filename: modo-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/modo-energy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Token\n  description: Public API token obtained from your Modo Energy account.\n  sources:\n  - openapi/modo-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modo-energy/refs/heads/main/authentication/modo-energy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Battery Storage
- Utilities
- Data
---
