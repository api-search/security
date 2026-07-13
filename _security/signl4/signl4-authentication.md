---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signl4 Authentication
name_suffix: Authentication
oauth_flows: []
overview: SIGNL4 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SIGNL4
provider_slug: signl4
scheme_count: 1
schemes:
- description: Team or webhook secret used to authorize REST API requests.
  in: header
  name: S4ApiKey
  parameter: X-S4-Api-Key
  sources:
  - openapi/signl4-openapi.yml
  type: apiKey
slug: signl4-authentication
source_filename: signl4-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signl4-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: S4ApiKey\n  type: apiKey\n  in: header\n  parameter: X-S4-Api-Key\n  description: Team or webhook secret used to authorize REST API requests.\n  sources:\n  - openapi/signl4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signl4/refs/heads/main/authentication/signl4-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alerting
- Incident Management
- On-Call
- Mobile Alerts
- Notifications
- DevOps
- IT Operations
- Monitoring
---
