---
api_key_in:
- header
api_specs:
- filename: skydio-openapi.yml
  format: yaml
  label: Skydio Cloud API
  slug: skydio-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydio/refs/heads/main/openapi/skydio-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Skydio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skydio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skydio
provider_slug: skydio
scheme_count: 1
schemes:
- description: Skydio Cloud API token. Generate in Skydio Cloud under Settings > API Tokens. Treat the token secret like a password.
  in: header
  name: ApiTokenAuth
  parameter: Authorization
  sources:
  - openapi/skydio-openapi.yml
  type: apiKey
slug: skydio-authentication
source_filename: skydio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/skydio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Skydio Cloud API token. Generate in Skydio Cloud under Settings > API Tokens.\n    Treat the token secret like a password.\n  sources:\n  - openapi/skydio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydio/refs/heads/main/authentication/skydio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Autonomous Systems
- Defense
- Drones
- Enterprise
- Fleet Management
- Public Safety
- Robotics
- Unmanned Aerial Vehicles
---
