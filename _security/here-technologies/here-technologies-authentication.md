---
api_key_in:
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Here Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: HERE Technologies secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HERE Technologies
provider_slug: here-technologies
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/here-technologies-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/here-technologies-openapi.yml
  type: http
slug: here-technologies-authentication
source_filename: here-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/here-technologies-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/here-technologies-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/here-technologies-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/authentication/here-technologies-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Maps
- Geocoding
- Routing
- Location Services
- Traffic
- HD Live Map
- Automotive
- Fleet
---
