---
api_key_in:
- header
api_specs:
- filename: curai-partner-openapi.json
  format: json
  label: Curai Partner API
  slug: curai-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/openapi/curai-partner-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Curai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Curai
provider_slug: curai
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/curai-partner-openapi.json
  type: apiKey
slug: curai-authentication
source_filename: curai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/curai-partner-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/curai-partner-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/authentication/curai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health
- Healthcare
- Telemedicine
- Telehealth
- Primary Care
- Digital Health
- Patient Engagement
- Partner API
- SDK
---
