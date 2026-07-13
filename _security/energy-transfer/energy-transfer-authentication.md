---
api_key_in: []
api_specs:
- filename: energy-transfer-messenger-api-openapi.yml
  format: yaml
  label: Energy Transfer Messenger+ API
  slug: messenger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-transfer/refs/heads/main/openapi/energy-transfer-messenger-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Energy Transfer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Energy Transfer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Energy Transfer
provider_slug: energy-transfer
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/energy-transfer-messenger-api-openapi.yml
  type: http
slug: energy-transfer-authentication
source_filename: energy-transfer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/energy-transfer-messenger-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/energy-transfer-messenger-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-transfer/refs/heads/main/authentication/energy-transfer-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Pipelines
- Midstream
- Gas Scheduling
- Fortune 100
---
