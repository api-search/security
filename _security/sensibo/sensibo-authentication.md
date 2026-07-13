---
api_key_in:
- query
api_specs:
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Users API
  slug: sensibo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Devices API
  slug: sensibo-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo AC States API
  slug: sensibo-ac-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Measurements API
  slug: sensibo-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Historical Data API
  slug: sensibo-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Climate React API
  slug: sensibo-climate-react-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Schedules API
  slug: sensibo-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Timers API
  slug: sensibo-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sensibo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensibo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sensibo
provider_slug: sensibo
scheme_count: 1
schemes:
- description: Per-account API key generated at https://home.sensibo.com/me/api and passed as the apiKey query parameter on every request.
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/sensibo-openapi.yml
  type: apiKey
slug: sensibo-authentication
source_filename: sensibo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sensibo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Per-account API key generated at https://home.sensibo.com/me/api and passed as\n    the apiKey query parameter on every request.\n  sources:\n  - openapi/sensibo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/authentication/sensibo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Smart Home
- IoT
- Air Conditioning
- HVAC
- Air Quality
- Climate Control
- Connected Devices
---
