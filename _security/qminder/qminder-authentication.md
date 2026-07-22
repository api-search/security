---
api_key_in:
- header
api_specs:
- filename: qminder-openapi-original.json
  format: json
  label: Qminder REST API
  slug: qminder-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qminder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qminder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qminder
provider_slug: qminder
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: X-Qminder-REST-API-Key
  sources:
  - openapi/qminder-openapi-original.json
  type: apiKey
slug: qminder-authentication
source_filename: qminder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qminder-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Qminder-REST-API-Key\n  sources:\n  - openapi/qminder-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/authentication/qminder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Queue Management
- Appointment Scheduling
- Visitor Management
- Customer Experience
- REST
- GraphQL
- Webhooks
- SaaS
---
