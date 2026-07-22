---
api_key_in: []
api_specs:
- filename: shyft-customer-openapi-original.json
  format: json
  label: Shyft Customer API
  slug: shyft-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shyft/refs/heads/main/openapi/shyft-customer-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shyft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shyft secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shyft
provider_slug: shyft
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shyft-customer-openapi-original.json
  type: http
- name: noauthAuth
  scheme: noauth
  sources:
  - openapi/shyft-customer-openapi-original.json
  type: http
slug: shyft-authentication
source_filename: shyft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shyft-customer-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/shyft-customer-openapi-original.json\n- name: noauthAuth\n  type: http\n  scheme: noauth\n  sources:\n  - openapi/shyft-customer-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shyft/refs/heads/main/authentication/shyft-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Workforce Management
- Employee Scheduling
- Shift Swapping
- Team Communication
- Hourly Workers
- Earned Wage Access
- HR Tech
- REST API
---
