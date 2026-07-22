---
api_key_in:
- header
api_specs:
- filename: upguard-cyberrisk-openapi-original.json
  format: json
  label: UpGuard CyberRisk API
  slug: upguard-cyberrisk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-cyberrisk-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Upguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpGuard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpGuard
provider_slug: upguard
scheme_count: 1
schemes:
- in: header
  name: API key in header
  parameter: Authorization
  sources:
  - openapi/upguard-cyberrisk-openapi-original.json
  type: apiKey
slug: upguard-authentication
source_filename: upguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/upguard-cyberrisk-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API key in header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/upguard-cyberrisk-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/authentication/upguard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Third-Party Risk Management
- Attack Surface Management
- Vendor Risk
- Security Ratings
- Data Leaks
- Threat Intelligence
---
