---
api_key_in: []
api_specs:
- filename: documentation
  format: yaml
  label: ProcessMaker Platform RESTful API
  slug: processmaker-platform-api
  spec_type: OpenAPI
  url: https://{organization}.processmaker.net/api/documentation
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Processmaker Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProcessMaker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProcessMaker
provider_slug: processmaker
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/processmaker-platform-api-openapi.yml
  type: http
slug: processmaker-authentication
source_filename: processmaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/processmaker-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/processmaker-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/authentication/processmaker-authentication.yml
summary_line: http · 1 scheme
tags:
- BPM
- Business Process Management
- Workflow Automation
- BPMN 2.0
- Low-Code
- Intelligent Automation
- Process Design
- Case Management
- Task Management
- Enterprise Integration
---
