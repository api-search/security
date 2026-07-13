---
api_key_in: []
api_specs:
- filename: cloudquery-openapi.json
  format: json
  label: CloudQuery Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudquery/refs/heads/main/openapi/cloudquery-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudquery Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudQuery secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CloudQuery
provider_slug: cloudquery
scheme_count: 3
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudquery-openapi.json
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/cloudquery-openapi.json
  type: http
- name: cookieAuth
  scheme: cookie
  sources:
  - openapi/cloudquery-openapi.json
  type: http
slug: cloudquery-authentication
source_filename: cloudquery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudquery-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cloudquery-openapi.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cloudquery-openapi.json\n- name: cookieAuth\n  type: http\n  scheme: cookie\n  sources:\n  - openapi/cloudquery-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudquery/refs/heads/main/authentication/cloudquery-authentication.yml
summary_line: http · 3 schemes
tags:
- Cloud Infrastructure
- Cloud Asset Inventory
- CSPM
- Cloud Governance
- FinOps
- Data Integration
- Platform Engineering
---
