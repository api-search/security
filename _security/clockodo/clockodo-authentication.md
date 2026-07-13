---
api_key_in:
- header
api_specs:
- filename: clockodo-openapi.yml
  format: yaml
  label: Clockodo API
  slug: clockodo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clockodo/refs/heads/main/openapi/clockodo-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clockodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clockodo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clockodo
provider_slug: clockodo
scheme_count: 2
schemes:
- description: Per-user API key. Must be paired with the X-ClockodoApiUser header carrying the user's email address.
  in: header
  name: clockodoApiKey
  parameter: X-ClockodoApiKey
  sources:
  - openapi/clockodo-openapi.yml
  type: apiKey
- description: HTTP Basic auth using the user's email as the username and the API key as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/clockodo-openapi.yml
  type: http
slug: clockodo-authentication
source_filename: clockodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clockodo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: clockodoApiKey\n  type: apiKey\n  in: header\n  parameter: X-ClockodoApiKey\n  description: Per-user API key. Must be paired with the X-ClockodoApiUser header carrying the\n    user's email address.\n  sources:\n  - openapi/clockodo-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using the user's email as the username and the API key as the\n    password.\n  sources:\n  - openapi/clockodo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockodo/refs/heads/main/authentication/clockodo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Absence Management
- Billing
- Project Management
- Stop Clock
- Time Tracking
- Timesheets
---
