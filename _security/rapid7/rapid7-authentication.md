---
api_key_in: []
api_specs:
- filename: insightidr-openapi.json
  format: json
  label: Rapid7 InsightIDR API
  slug: insightidr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapid7/refs/heads/main/openapi/insightidr-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rapid7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rapid7 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rapid7
provider_slug: rapid7
scheme_count: 1
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/insightvm-console-swagger.json
  type: http
slug: rapid7-authentication
source_filename: rapid7-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/insightvm-console-swagger.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/insightvm-console-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapid7/refs/heads/main/authentication/rapid7-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Vulnerability Management
- SIEM
- XDR
- Cloud Security
- SOAR
- Application Security
---
