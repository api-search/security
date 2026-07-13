---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zenduty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenduty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zenduty
provider_slug: zenduty
scheme_count: 1
schemes:
- bearerFormat: Token <api_key>
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zenduty-openapi.json
  type: http
slug: zenduty-authentication
source_filename: zenduty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenduty-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Token <api_key>\n  sources:\n  - openapi/zenduty-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenduty/refs/heads/main/authentication/zenduty-authentication.yml
summary_line: http · 1 scheme
tags:
- Incident Management
- On-Call
- Alerting
- SRE
- DevOps
- Observability
---
