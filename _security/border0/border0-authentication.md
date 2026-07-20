---
api_key_in:
- header
api_specs:
- filename: border0-openapi.json
  format: json
  label: Border0 API
  slug: border0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Border0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Border0 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Border0
provider_slug: border0
scheme_count: 1
schemes:
- in: header
  name: Border0_Token
  parameter: Authorization
  sources:
  - openapi/border0-openapi.json
  type: apiKey
slug: border0-authentication
source_filename: border0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/border0-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Border0_Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/border0-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/authentication/border0-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Zero Trust
- Network Access
- Security
- Identity and Access Management
- Infrastructure
- VPN
- SSH
- Databases
- Kubernetes
- Company
---
