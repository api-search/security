---
api_key_in:
- header
api_specs:
- filename: memfault-openapi.yml
  format: yaml
  label: Memfault Cloud REST API
  slug: memfault-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Memfault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memfault secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Memfault
provider_slug: memfault
scheme_count: 3
schemes:
- bearerFormat: token
  description: 'Organization Auth Token. Use "Authorization: Bearer [example key]" for automation

    and full API access.'
  name: orgAuthToken
  scheme: bearer
  sources:
  - openapi/memfault-openapi.yml
  type: http
- description: Email + password or Email + user API key via HTTP Basic auth.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/memfault-openapi.yml
  type: http
- description: 'Memfault Project Key used by devices and ingestion endpoints (chunks,

    latest release lookup, events, coredumps).'
  in: header
  name: projectKey
  parameter: Memfault-Project-Key
  sources:
  - openapi/memfault-openapi.yml
  type: apiKey
slug: memfault-authentication
source_filename: memfault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/memfault-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: orgAuthToken\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: |-\n    Organization Auth Token. Use \"Authorization: Bearer [example key]\" for automation\n    and full API access.\n  sources:\n  - openapi/memfault-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Email + password or Email + user API key via HTTP Basic auth.\n  sources:\n  - openapi/memfault-openapi.yml\n- name: projectKey\n  type: apiKey\n  in: header\n  parameter: Memfault-Project-Key\n  description: |-\n    Memfault Project Key used by devices and ingestion endpoints (chunks,\n    latest release lookup, events, coredumps).\n  sources:\n  - openapi/memfault-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/authentication/memfault-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Alerts
- Android
- Crash Reporting
- Device Management
- Embedded
- Embedded Linux
- Firmware
- IoT
- Logging
- MCU
- Metrics
- Observability
- OTA
- Reliability
---
