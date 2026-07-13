---
api_key_in:
- header
api_specs:
- filename: stacker-openapi.yml
  format: yaml
  label: Stacker API
  slug: stacker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacker/refs/heads/main/openapi/stacker-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stacker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stacker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stacker
provider_slug: stacker
scheme_count: 1
schemes:
- description: Personal integration key from Account Settings > Integrations
  in: header
  name: IntegrationKey
  parameter: X-Integration-Key
  sources:
  - openapi/stacker-openapi.yml
  type: apiKey
slug: stacker-authentication
source_filename: stacker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stacker-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: IntegrationKey\n  type: apiKey\n  in: header\n  parameter: X-Integration-Key\n  description: Personal integration key from Account Settings > Integrations\n  sources:\n  - openapi/stacker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacker/refs/heads/main/authentication/stacker-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Development
- Low-Code
- No-Code
- Portals
- Workflow Automation
---
