---
api_key_in:
- cookie
api_specs:
- filename: us-space-command-space-track-openapi.yml
  format: yaml
  label: Space-Track.org REST API
  slug: space-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/openapi/us-space-command-space-track-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Space Comman Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Space Command secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: US Space Command
provider_slug: us-space-comman
scheme_count: 1
schemes:
- description: Session cookie obtained after successful login via POST /ajaxauth/login
  in: cookie
  name: sessionCookie
  parameter: chocolatechip
  sources:
  - openapi/us-space-command-space-track-openapi.yml
  type: apiKey
slug: us-space-comman-authentication
source_filename: us-space-comman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/us-space-command-space-track-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: chocolatechip\n  description: Session cookie obtained after successful login via POST /ajaxauth/login\n  sources:\n  - openapi/us-space-command-space-track-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/authentication/us-space-comman-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Space
- Space Situational Awareness
- Satellite Tracking
- Open Data
---
