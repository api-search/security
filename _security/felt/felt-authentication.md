---
api_key_in: []
api_specs:
- filename: felt-felt-rest-api-openapi.yml
  format: yaml
  label: Felt REST API
  slug: felt-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-felt-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Felt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Felt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Felt
provider_slug: felt
scheme_count: 1
schemes:
- bearerFormat: YOUR_API_KEY
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/felt-felt-rest-api-openapi.yml
  type: http
slug: felt-authentication
source_filename: felt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/felt-felt-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: YOUR_API_KEY\n  sources:\n  - openapi/felt-felt-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/authentication/felt-authentication.yml
summary_line: http · 1 scheme
tags:
- Maps
- GIS
- Geospatial
- Collaborative
- Mapping
- Layers
- Embedding
---
