---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Itch.io API
  slug: itch-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Itch Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Itch.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Itch.io
provider_slug: itch-io
scheme_count: 1
schemes:
- description: API key or JWT token issued by itch.io
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: itch-io-authentication
source_filename: itch-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key or JWT token issued by itch.io\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/authentication/itch-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Games
- Indie Games
- Game Distribution
- Game Marketplace
- Developers
---
