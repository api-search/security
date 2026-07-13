---
api_key_in:
- header
api_specs:
- filename: simscale-openapi.yml
  format: yaml
  label: SimScale REST API
  slug: simscale-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Simscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimScale secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimScale
provider_slug: simscale
scheme_count: 1
schemes:
- description: SimScale API key. Generate in your SimScale account settings.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/simscale-openapi.yml
  type: apiKey
slug: simscale-authentication
source_filename: simscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simscale-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: SimScale API key. Generate in your SimScale account settings.\n  sources:\n  - openapi/simscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/authentication/simscale-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CAE
- CFD
- FEA
- Simulation
- Engineering
---
