---
api_key_in:
- header
api_specs:
- filename: nected-openapi.yml
  format: yaml
  label: Nected
  slug: nected
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nected/refs/heads/main/openapi/nected-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nected Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nected secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nected
provider_slug: nected
scheme_count: 1
schemes:
- in: header
  name: NectedApiKey
  parameter: nected-api-key
  sources:
  - openapi/nected-openapi.yml
  type: apiKey
slug: nected-authentication
source_filename: nected-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nected-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: NectedApiKey\n  type: apiKey\n  in: header\n  parameter: nected-api-key\n  sources:\n  - openapi/nected-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nected/refs/heads/main/authentication/nected-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Low-Code
- Workflow Automation
- Decision Engine
- Business Rules
---
