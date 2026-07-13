---
api_key_in: []
api_specs:
- filename: subex-revenue-assurance-openapi.yml
  format: yaml
  label: Subex Revenue Assurance & Fraud Management API
  slug: subex-revenue-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-revenue-assurance-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Subex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Subex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Subex
provider_slug: subex
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/subex-revenue-assurance-openapi.yml
  type: http
slug: subex-authentication
source_filename: subex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/subex-revenue-assurance-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/subex-revenue-assurance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/authentication/subex-authentication.yml
summary_line: http · 1 scheme
tags:
- Telecom
- Revenue Assurance
- Fraud Management
- Analytics
- BSS/OSS
---
