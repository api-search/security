---
api_key_in: []
api_specs:
- filename: sense-authentication-api-openapi.yml
  format: yaml
  label: Sense Authentication API
  slug: sense-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-authentication-api-openapi.yml
- filename: sense-devices-api-openapi.yml
  format: yaml
  label: Sense Devices API
  slug: sense-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-devices-api-openapi.yml
- filename: sense-history-api-openapi.yml
  format: yaml
  label: Sense History API
  slug: sense-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-history-api-openapi.yml
- filename: sense-monitors-api-openapi.yml
  format: yaml
  label: Sense Monitors API
  slug: sense-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-monitors-api-openapi.yml
- filename: sense-users-api-openapi.yml
  format: yaml
  label: Sense Users API
  slug: sense-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sense secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sense
provider_slug: sense
scheme_count: 1
schemes:
- description: 'Bearer token obtained from the /authenticate or /renew endpoints. Include as "Authorization: bearer <access_token>" header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sense-sense-client-api-openapi.yml
  type: http
slug: sense-authentication
source_filename: sense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sense-sense-client-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token obtained from the /authenticate or /renew endpoints. Include as\n    \"Authorization: bearer <access_token>\" header.'\n  sources:\n  - openapi/sense-sense-client-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/authentication/sense-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Home Energy Monitoring
- IoT
- Smart Home
- Electricity
- Solar
- Device Detection
- Real-Time Data
- Climate Tech
---
