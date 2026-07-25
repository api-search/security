---
api_key_in:
- header
api_specs:
- filename: memfault-organizations-api-openapi.yml
  format: yaml
  label: Memfault Organizations API
  slug: memfault-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-organizations-api-openapi.yml
- filename: memfault-projects-api-openapi.yml
  format: yaml
  label: Memfault Projects API
  slug: memfault-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-projects-api-openapi.yml
- filename: memfault-devices-api-openapi.yml
  format: yaml
  label: Memfault Devices API
  slug: memfault-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-devices-api-openapi.yml
- filename: memfault-issues-api-openapi.yml
  format: yaml
  label: Memfault Issues API
  slug: memfault-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-issues-api-openapi.yml
- filename: memfault-chunks-api-openapi.yml
  format: yaml
  label: Memfault Chunks Ingestion API
  slug: memfault-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-chunks-api-openapi.yml
- filename: memfault-auth-api-openapi.yml
  format: yaml
  label: Memfault Auth API
  slug: memfault-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-auth-api-openapi.yml
- filename: memfault-chunks-api-openapi.yml
  format: yaml
  label: Memfault Chunks API
  slug: memfault-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-chunks-api-openapi.yml
- filename: memfault-cohorts-api-openapi.yml
  format: yaml
  label: Memfault Cohorts API
  slug: memfault-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-cohorts-api-openapi.yml
- filename: memfault-deployments-api-openapi.yml
  format: yaml
  label: Memfault Deployments API
  slug: memfault-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-deployments-api-openapi.yml
- filename: memfault-devices-api-openapi.yml
  format: yaml
  label: Memfault Devices API
  slug: memfault-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-devices-api-openapi.yml
- filename: memfault-files-api-openapi.yml
  format: yaml
  label: Memfault Files API
  slug: memfault-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-files-api-openapi.yml
- filename: memfault-issues-api-openapi.yml
  format: yaml
  label: Memfault Issues API
  slug: memfault-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-issues-api-openapi.yml
- filename: memfault-organizations-api-openapi.yml
  format: yaml
  label: Memfault Organizations API
  slug: memfault-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-organizations-api-openapi.yml
- filename: memfault-projects-api-openapi.yml
  format: yaml
  label: Memfault Projects API
  slug: memfault-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-projects-api-openapi.yml
- filename: memfault-releases-api-openapi.yml
  format: yaml
  label: Memfault Releases API
  slug: memfault-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-releases-api-openapi.yml
- filename: memfault-software-api-openapi.yml
  format: yaml
  label: Memfault Software API
  slug: memfault-software-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-software-api-openapi.yml
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
