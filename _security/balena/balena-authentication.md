---
api_key_in: []
api_specs:
- filename: balena-openapi.yml
  format: yaml
  label: Balena Cloud API
  slug: balena-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balena/refs/heads/main/openapi/balena-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Balena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Balena secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Balena
provider_slug: balena
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Session token or named API key supplied as

    `Authorization: Bearer <token>`. Create named API keys at

    https://dashboard.balena-cloud.com/preferences/access-tokens.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/balena-openapi.yml
  type: http
slug: balena-authentication
source_filename: balena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/balena-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Session token or named API key supplied as\n    `Authorization: Bearer <token>`. Create named API keys at\n    https://dashboard.balena-cloud.com/preferences/access-tokens.\n  sources:\n  - openapi/balena-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balena/refs/heads/main/authentication/balena-authentication.yml
summary_line: http · 1 scheme
tags:
- Containers
- Device Management
- Edge
- Embedded Linux
- Fleet Management
- IoT
- OTA
- Provisioning
- Releases
---
