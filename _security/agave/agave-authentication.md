---
api_key_in:
- header
api_specs:
- filename: agave-unified-api-openapi.yml
  format: yaml
  label: Agave Unified Construction API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-unified-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agave
provider_slug: agave
scheme_count: 1
schemes:
- description: Agave API key for authentication.
  in: header
  name: apiKey
  parameter: API-Key
  sources:
  - openapi/agave-unified-api-openapi.yml
  type: apiKey
slug: agave-authentication
source_filename: agave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agave-unified-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: Agave API key for authentication.\n  sources:\n  - openapi/agave-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/authentication/agave-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accounting
- Construction
- Integration
---
