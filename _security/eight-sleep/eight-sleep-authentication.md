---
api_key_in: []
api_specs:
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Authentication API
  slug: eight-sleep-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep User API
  slug: eight-sleep-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Device API
  slug: eight-sleep-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Temperature API
  slug: eight-sleep-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Trends API
  slug: eight-sleep-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Base API
  slug: eight-sleep-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Alarms API
  slug: eight-sleep-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eight Sleep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eight Sleep secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eight Sleep
provider_slug: eight-sleep
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token issued by POST /v1/tokens on auth-api.8slp.net. Unofficial.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eight-sleep-openapi.yml
  type: http
slug: eight-sleep-authentication
source_filename: eight-sleep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eight-sleep-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token issued by POST /v1/tokens on auth-api.8slp.net. Unofficial.\n  sources:\n  - openapi/eight-sleep-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/authentication/eight-sleep-authentication.yml
summary_line: http · 1 scheme
tags:
- Sleep
- IoT
- Smart Home
- Wearables
- Health
- Unofficial
---
