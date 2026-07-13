---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pandascore Authentication
name_suffix: Authentication
oauth_flows: []
overview: PandaScore secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PandaScore
provider_slug: pandascore
scheme_count: 1
schemes:
- description: Bearer token authentication using a PandaScore API token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pandascore-openapi.yml
  type: http
slug: pandascore-authentication
source_filename: pandascore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pandascore-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a PandaScore API token\n  sources:\n  - openapi/pandascore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/authentication/pandascore-authentication.yml
summary_line: http · 1 scheme
tags:
- Esports
- Odds
- Betting
- Live Data
- Stats
- Fantasy
- WebSocket
- REST
---
