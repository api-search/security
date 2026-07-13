---
api_key_in: []
api_specs:
- filename: zeebe-api.yml
  format: yaml
  label: Zeebe REST API
  slug: zeebe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zeebe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeebe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zeebe
provider_slug: zeebe
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zeebe-api.yml
  type: http
slug: zeebe-authentication
source_filename: zeebe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeebe-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zeebe-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/authentication/zeebe-authentication.yml
summary_line: http · 1 scheme
tags:
- BPMN
- Camunda
- Cloud Native
- Distributed Systems
- Java
- Microservices
- Process Automation
- Workflow Orchestration
---
