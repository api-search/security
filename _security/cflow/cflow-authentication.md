---
api_key_in:
- header
api_specs:
- filename: cflow-openapi.yml
  format: yaml
  label: Cflow Workflow API
  slug: cflow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/openapi/cflow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cflow secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cflow
provider_slug: cflow
scheme_count: 3
schemes:
- description: API key obtained from Cflow Dashboard under Admin > API Settings > Generate API key.
  in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/cflow-openapi.yml
  type: apiKey
- description: User key obtained from Cflow Profile > API Key > UserKey.
  in: header
  name: userKey
  parameter: userkey
  sources:
  - openapi/cflow-openapi.yml
  type: apiKey
- description: The Cflow account username.
  in: header
  name: username
  parameter: username
  sources:
  - openapi/cflow-openapi.yml
  type: apiKey
slug: cflow-authentication
source_filename: cflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key obtained from Cflow Dashboard under Admin > API Settings > Generate API\n    key.\n  sources:\n  - openapi/cflow-openapi.yml\n- name: userKey\n  type: apiKey\n  in: header\n  parameter: userkey\n  description: User key obtained from Cflow Profile > API Key > UserKey.\n  sources:\n  - openapi/cflow-openapi.yml\n- name: username\n  type: apiKey\n  in: header\n  parameter: username\n  description: The Cflow account username.\n  sources:\n  - openapi/cflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/authentication/cflow-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
---
