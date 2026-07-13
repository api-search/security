---
api_key_in: []
api_specs:
- filename: particle-cloud-api-openapi.yml
  format: yaml
  label: Particle Cloud API
  slug: particle-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle/refs/heads/main/openapi/particle-cloud-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Particle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Particle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Particle
provider_slug: particle
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token. Obtain via POST /oauth/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/particle-cloud-api-openapi.yml
  type: http
slug: particle-authentication
source_filename: particle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/particle-cloud-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token. Obtain via POST /oauth/token.\n  sources:\n  - openapi/particle-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle/refs/heads/main/authentication/particle-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Internet of Things
- Cellular
- Wi-Fi
- Bluetooth
- Device Management
- Firmware
- OTA Updates
- Fleet Management
- Hardware
- Embedded
---
