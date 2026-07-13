---
api_key_in:
- header
api_specs:
- filename: ilert-ilert-rest-api-openapi.yml
  format: yaml
  label: ilert REST API
  slug: ilert-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ilert/refs/heads/main/openapi/ilert-ilert-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ilert Authentication
name_suffix: Authentication
oauth_flows: []
overview: ilert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ilert
provider_slug: ilert
scheme_count: 1
schemes:
- description: The Bearer API key of your user <a href='/api-docs/#section/Authentication'>more info</a>.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/ilert-ilert-rest-api-openapi.yml
  type: apiKey
slug: ilert-authentication
source_filename: ilert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ilert-ilert-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The Bearer API key of your user <a href='/api-docs/#section/Authentication'>more\n    info</a>.\n  sources:\n  - openapi/ilert-ilert-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ilert/refs/heads/main/authentication/ilert-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Incident Management
- On-Call Alerting
- Alert Routing
- Escalation Policies
- On-Call Schedules
- Status Pages
- Heartbeat Monitoring
- Event Management
- DevOps
- SRE
- IT Operations
---
