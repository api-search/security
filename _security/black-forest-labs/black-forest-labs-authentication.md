---
api_key_in:
- header
api_specs:
- filename: black-forest-labs-openapi.yml
  format: yaml
  label: Flux Image Generation API
  slug: flux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-forest-labs/refs/heads/main/openapi/black-forest-labs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Black Forest Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Black Forest Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Black Forest Labs
provider_slug: black-forest-labs
scheme_count: 1
schemes:
- description: BFL API key.
  in: header
  name: apiKey
  parameter: x-key
  sources:
  - openapi/black-forest-labs-openapi.yml
  type: apiKey
slug: black-forest-labs-authentication
source_filename: black-forest-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/black-forest-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-key\n  description: BFL API key.\n  sources:\n  - openapi/black-forest-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-forest-labs/refs/heads/main/authentication/black-forest-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Image Generation
- Flux
- Open Weights
- BFL
---
