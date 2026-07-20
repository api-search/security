---
api_key_in:
- query
api_specs:
- filename: liquid-m-reporting-openapi.yml
  format: yaml
  label: LiquidM Reporting API
  slug: reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-reporting-openapi.yml
- filename: liquid-m-management-openapi.yml
  format: yaml
  label: LiquidM Management API
  slug: management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Liquid M Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liquid M secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Liquid M
provider_slug: liquid-m
scheme_count: 1
schemes:
- description: AUTH_TOKEN passed as a query parameter on every request, including POSTs.
  in: query
  name: authToken
  parameter: auth_token
  sources:
  - openapi/liquid-m-management-openapi.yml
  - openapi/liquid-m-reporting-openapi.yml
  type: apiKey
slug: liquid-m-authentication
source_filename: liquid-m-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/liquid-m-management-openapi.yml, openapi/liquid-m-reporting-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: authToken\n  type: apiKey\n  in: query\n  parameter: auth_token\n  description: AUTH_TOKEN passed as a query parameter on every request, including POSTs.\n  sources:\n  - openapi/liquid-m-management-openapi.yml\n  - openapi/liquid-m-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/authentication/liquid-m-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Advertising
- AdTech
- Demand-Side Platform
- Programmatic Advertising
- Mobile Advertising
- Reporting
- Analytics
- Campaign Management
- OpenRTB
---
