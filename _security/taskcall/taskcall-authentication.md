---
api_key_in:
- header
api_specs:
- filename: taskcall-openapi.yml
  format: yaml
  label: TaskCall Incidents API
  slug: incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskcall/refs/heads/main/openapi/taskcall-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Taskcall Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaskCall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TaskCall
provider_slug: taskcall
scheme_count: 1
schemes:
- description: 'API key formatted as: token <api_key>'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/taskcall-openapi.yml
  type: apiKey
slug: taskcall-authentication
source_filename: taskcall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taskcall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key formatted as: token <api_key>'\n  sources:\n  - openapi/taskcall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskcall/refs/heads/main/authentication/taskcall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Incident Management
- On-Call
- Alerting
- DevOps
- SRE
- ITSM
---
