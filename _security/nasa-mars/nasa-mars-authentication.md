---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: nasa-mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-mars/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nasa Mars Authentication
name_suffix: Authentication
oauth_flows: []
overview: NASA Mars Rovers secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NASA Mars Rovers
provider_slug: nasa-mars
scheme_count: 1
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: nasa-mars-authentication
source_filename: nasa-mars-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-mars/refs/heads/main/authentication/nasa-mars-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NASA
- Mars
- Rovers
- Photos
- Images
- Space
- Planetary Science
- Open Data
---
