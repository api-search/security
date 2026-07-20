---
api_key_in: []
api_specs:
- filename: hex-openapi-original.json
  format: json
  label: Hex External API
  slug: hex-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hex
provider_slug: hex
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hex-openapi-original.json
  type: http
slug: hex-authentication
source_filename: hex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hex-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hex-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/authentication/hex-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Analytics
- Data Science
- Notebooks
- Business Intelligence
- Data Apps
- AI
- Agents
- Semantic Layer
- Developer Tools
---
