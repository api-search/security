---
api_key_in: []
api_specs:
- filename: recraft-openapi.yml
  format: yaml
  label: Recraft API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recraft/refs/heads/main/openapi/recraft-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Recraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recraft secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recraft
provider_slug: recraft
scheme_count: 1
schemes:
- description: Bearer token authentication using a Recraft API token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/recraft-openapi.yml
  type: http
slug: recraft-authentication
source_filename: recraft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/recraft-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a Recraft API token.\n  sources:\n  - openapi/recraft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recraft/refs/heads/main/authentication/recraft-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Image Generation
- Design
- Vector
- Style
---
