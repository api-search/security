---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Airport Gap REST API
  slug: airport-gap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airport-gap/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airport Gap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airport Gap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airport Gap
provider_slug: airport-gap
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'Token-based authentication. Include the token generated from POST /tokens. Header format: Authorization: Bearer token=<Your Airport Gap Token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: airport-gap-authentication
source_filename: airport-gap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: 'Token-based authentication. Include the token generated from POST /tokens. Header\n    format: Authorization: Bearer token=<Your Airport Gap Token>'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airport-gap/refs/heads/main/authentication/airport-gap-authentication.yml
summary_line: http · 1 scheme
tags:
- Airports
- Aviation
- Transportation
- IATA
- ICAO
- Distance Calculation
- Geolocation
---
