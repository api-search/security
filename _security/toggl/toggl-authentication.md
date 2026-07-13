---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toggl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toggl Track secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toggl Track
provider_slug: toggl
scheme_count: 1
schemes:
- description: 'HTTP Basic auth. Username is the API token from Toggl profile,

    password is the literal string `api_token`.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/toggl-openapi.yml
  type: http
slug: toggl-authentication
source_filename: toggl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toggl-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth. Username is the API token from Toggl profile,\n    password is the literal string `api_token`.\n  sources:\n  - openapi/toggl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toggl/refs/heads/main/authentication/toggl-authentication.yml
summary_line: http · 1 scheme
tags:
- Time Tracking
- Productivity
- Project Management
- Billing
- Reporting
- Workforce Management
---
