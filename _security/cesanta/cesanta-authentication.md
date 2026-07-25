---
api_key_in: []
api_specs:
- filename: cesanta-data-api-openapi.yml
  format: yaml
  label: Cesanta Data API
  slug: cesanta-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-data-api-openapi.yml
- filename: cesanta-devices-api-openapi.yml
  format: yaml
  label: Cesanta Devices API
  slug: cesanta-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-devices-api-openapi.yml
- filename: cesanta-keys-api-openapi.yml
  format: yaml
  label: Cesanta Keys API
  slug: cesanta-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-keys-api-openapi.yml
- filename: cesanta-logs-api-openapi.yml
  format: yaml
  label: Cesanta Logs API
  slug: cesanta-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-logs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cesanta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cesanta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cesanta
provider_slug: cesanta
scheme_count: 1
schemes:
- description: mDash API key sent as an HTTP bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cesanta-mdash-openapi.yml
  type: http
slug: cesanta-authentication
source_filename: cesanta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cesanta-mdash-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: mDash API key sent as an HTTP bearer token.\n  sources:\n  - openapi/cesanta-mdash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/authentication/cesanta-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- IoT
- Embedded
- Device Management
- Firmware
- OTA
- Networking
- MQTT
---
