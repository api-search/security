---
api_key_in:
- header
api_specs:
- filename: keeptrack-catalog-api-openapi.yml
  format: yaml
  label: KeepTrack Catalog API
  slug: keeptrack-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/openapi/keeptrack-catalog-api-openapi.yml
- filename: keeptrack-orbits-api-openapi.yml
  format: yaml
  label: KeepTrack Orbits API
  slug: keeptrack-orbits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/openapi/keeptrack-orbits-api-openapi.yml
- filename: keeptrack-positions-api-openapi.yml
  format: yaml
  label: KeepTrack Positions API
  slug: keeptrack-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/openapi/keeptrack-positions-api-openapi.yml
- filename: keeptrack-satellites-api-openapi.yml
  format: yaml
  label: KeepTrack Satellites API
  slug: keeptrack-satellites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/openapi/keeptrack-satellites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Keeptrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeepTrack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KeepTrack
provider_slug: keeptrack
scheme_count: 1
schemes:
- description: Free API key issued from https://keeptrack.space.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/keeptrack-openapi.yml
  type: apiKey
slug: keeptrack-authentication
source_filename: keeptrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keeptrack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Free API key issued from https://keeptrack.space.\n  sources:\n  - openapi/keeptrack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/authentication/keeptrack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Satellites
- Space
---
