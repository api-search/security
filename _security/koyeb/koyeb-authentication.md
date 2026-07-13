---
api_key_in:
- header
api_specs:
- filename: koyeb-openapi.json
  format: json
  label: Koyeb API
  slug: koyeb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koyeb/refs/heads/main/openapi/koyeb-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Koyeb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koyeb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koyeb
provider_slug: koyeb
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/koyeb-openapi.json
  type: apiKey
slug: koyeb-authentication
source_filename: koyeb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/koyeb-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/koyeb-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koyeb/refs/heads/main/authentication/koyeb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Platform
- Deployment
- PaaS
- Serverless
---
