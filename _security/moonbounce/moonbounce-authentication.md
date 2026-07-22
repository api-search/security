---
api_key_in: []
api_specs:
- filename: moonbounce-openapi-original.json
  format: json
  label: Clavata Public API v1
  slug: clavata-public-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonbounce/refs/heads/main/openapi/moonbounce-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moonbounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moonbounce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moonbounce
provider_slug: moonbounce
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Bearer_Token
  scheme: bearer
  sources:
  - openapi/moonbounce-openapi-original.json
  type: http
slug: moonbounce-authentication
source_filename: moonbounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/moonbounce-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer_Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/moonbounce-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonbounce/refs/heads/main/authentication/moonbounce-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- Content Moderation
- Trust And Safety
- AI Governance
- Policy Enforcement
- Content Evaluation
---
