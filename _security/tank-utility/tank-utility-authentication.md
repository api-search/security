---
api_key_in:
- query
api_specs:
- filename: tank-utility-devices-openapi.yml
  format: yaml
  label: Tank Utility Propane Monitor API
  slug: tank-utility-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tank-utility/refs/heads/main/openapi/tank-utility-devices-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tank Utility Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tank Utility secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tank Utility
provider_slug: tank-utility
scheme_count: 2
schemes:
- description: HTTP Basic authentication using the Tank Utility account email (username) and password. Used only by getToken.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tank-utility-devices-openapi.yml
  type: http
- description: Short-lived API token obtained from getToken, passed as the `token` query parameter. Expires after ~24 hours.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/tank-utility-devices-openapi.yml
  type: apiKey
slug: tank-utility-authentication
source_filename: tank-utility-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tank-utility-devices-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the Tank Utility account email (username) and\n    password. Used only by getToken.\n  sources:\n  - openapi/tank-utility-devices-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Short-lived API token obtained from getToken, passed as the `token` query parameter.\n    Expires after ~24 hours.\n  sources:\n  - openapi/tank-utility-devices-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tank-utility/refs/heads/main/authentication/tank-utility-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Propane
- Tank Monitoring
- IoT
- Fuel Delivery
- Telemetry
- Energy
- Sensors
- Company
---
