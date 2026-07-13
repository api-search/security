---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: NASA NeoWs API
  slug: nasa-neows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-neows/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nasa Neows Authentication
name_suffix: Authentication
oauth_flows: []
overview: NASA NeoWs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NASA NeoWs
provider_slug: nasa-neows
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: nasa-neows-authentication
source_filename: nasa-neows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-neows/refs/heads/main/authentication/nasa-neows-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NASA
- Asteroids
- Near Earth Objects
- Space
- Science
- Open Data
- Planetary Defense
---
