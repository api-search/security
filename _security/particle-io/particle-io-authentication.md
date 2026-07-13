---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Particle Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Particle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Particle
provider_slug: particle-io
scheme_count: 1
schemes:
- bearerFormat: OAuth2 access token
  description: 'Pass `Authorization: Bearer {access_token}`. Tokens are issued via

    `POST /oauth/token`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/particle-io-openapi.yml
  type: http
slug: particle-io-authentication
source_filename: particle-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/particle-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  description: |-\n    Pass `Authorization: Bearer {access_token}`. Tokens are issued via\n    `POST /oauth/token`.\n  sources:\n  - openapi/particle-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-io/refs/heads/main/authentication/particle-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Cellular
- Cloud Functions
- Connectivity
- Device Management
- Edge
- Firmware
- Fleet Management
- IoT
- OTA
- Webhooks
- Wi-Fi
---
