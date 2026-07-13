---
api_key_in: []
api_specs:
- filename: tray-io-platform-api-openapi.yml
  format: yaml
  label: Tray.io Platform API
  slug: tray-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-io/refs/heads/main/openapi/tray-io-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tray Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tray.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tray.io
provider_slug: tray-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tray-io-platform-api-openapi.yml
  type: http
slug: tray-io-authentication
source_filename: tray-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tray-io-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tray-io-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-io/refs/heads/main/authentication/tray-io-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- API Aggregation
- Automation
- Connectors
- Integration
- iPaaS
- Workflow Automation
---
