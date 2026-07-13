---
api_key_in: []
api_specs:
- filename: cronitor-monitors-api-openapi.yml
  format: yaml
  label: Cronitor Monitors API
  slug: monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-monitors-api-openapi.yml
- filename: cronitor-telemetry-api-openapi.yml
  format: yaml
  label: Cronitor Telemetry API
  slug: telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-telemetry-api-openapi.yml
- filename: cronitor-groups-notifications-api-openapi.yml
  format: yaml
  label: Cronitor Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-groups-notifications-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cronitor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cronitor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cronitor
provider_slug: cronitor
scheme_count: 1
schemes:
- description: Use your Cronitor API key as the username; leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cronitor-groups-notifications-api-openapi.yml
  - openapi/cronitor-monitors-api-openapi.yml
  type: http
slug: cronitor-authentication
source_filename: cronitor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cronitor-groups-notifications-api-openapi.yml, openapi/cronitor-monitors-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your Cronitor API key as the username; leave the password blank.\n  sources:\n  - openapi/cronitor-groups-notifications-api-openapi.yml\n  - openapi/cronitor-monitors-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/authentication/cronitor-authentication.yml
summary_line: http · 1 scheme
tags:
- Monitoring
- Cron Jobs
- Scheduled Tasks
- Alerting
- Uptime
- Telemetry
- Status Pages
---
