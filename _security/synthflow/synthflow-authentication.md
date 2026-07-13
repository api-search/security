---
api_key_in: []
api_specs:
- filename: synthflow-openapi.json
  format: json
  label: Synthflow Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synthflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synthflow
provider_slug: synthflow
scheme_count: 1
schemes:
- name: sec0
  scheme: bearer
  sources:
  - openapi/synthflow-openapi.json
  type: http
slug: synthflow-authentication
source_filename: synthflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synthflow-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: sec0\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/synthflow-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/authentication/synthflow-authentication.yml
summary_line: http · 1 scheme
tags:
- Voice
- Voice Agents
- No-Code
- Telephony
- Phone
- Outbound
- Inbound
- CRM
- Webhooks
- Custom Actions
- HIPAA
- SOC 2
---
