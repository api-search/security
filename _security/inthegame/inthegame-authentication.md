---
api_key_in:
- header
api_specs:
- filename: inthegame-openapi.yml
  format: yaml
  label: Inthegame API
  slug: inthegame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inthegame/refs/heads/main/openapi/inthegame-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inthegame Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inthegame secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inthegame
provider_slug: inthegame
scheme_count: 1
schemes:
- description: Admin API token issued after login to the admin panel (https://admintest.inthegame.io/); sent in the Authorization header.
  in: header
  name: AdminToken
  parameter: Authorization
  sources:
  - openapi/inthegame-openapi.yml
  type: apiKey
slug: inthegame-authentication
source_filename: inthegame-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/inthegame-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AdminToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Admin API token issued after login to the admin panel (https://admintest.inthegame.io/);\n    sent in the Authorization header.\n  sources:\n  - openapi/inthegame-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inthegame/refs/heads/main/authentication/inthegame-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Streaming
- CTV
- OTT
- Video
- Engagement
- Interactive
- Gamification
- Sports
- Real-time
---
