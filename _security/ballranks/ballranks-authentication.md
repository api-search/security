---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ballranks-rankings-and-projections-api-openapi.yml
  format: yaml
  label: Ball Ranks Rankings and projections API
  slug: ballranks-rankings-and-projections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballranks/refs/heads/main/openapi/ballranks-rankings-and-projections-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ballranks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ball Ranks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ball Ranks
provider_slug: ballranks
scheme_count: 1
schemes:
- bearerFormat: Ball Ranks API key
  description: Optional Ball Ranks API key. Anonymous requests receive lower limits and Model v0 access only.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ballranks-openapi.json
  type: http
slug: ballranks-authentication
source_filename: ballranks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/ballranks-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Ball Ranks API key\n  description: Optional Ball Ranks API key. Anonymous requests receive lower limits and Model\n    v0 access only.\n  sources:\n  - openapi/ballranks-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballranks/refs/heads/main/authentication/ballranks-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fantasy Sports
- AI
- Rankings
- Projections
---
