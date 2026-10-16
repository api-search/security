---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coala-life-patientsessions-api-openapi.yml
  format: yaml
  label: Coala Life Patient Sessions API
  slug: coala-life-patientsessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-patientsessions-api-openapi.yml
- filename: coala-life-platform-api-api-openapi.yml
  format: yaml
  label: Coala Life Platform.Api API
  slug: coala-life-platform-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-platform-api-api-openapi.yml
- filename: coala-life-sessions-api-openapi.yml
  format: yaml
  label: Coala Life Sessions API
  slug: coala-life-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-sessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coala Life Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coala Life secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coala Life
provider_slug: coala-life
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/coala-life-openapi.json
  type: http
slug: coala-life-authentication
source_filename: coala-life-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/coala-life-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/coala-life-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/authentication/coala-life-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Cardiology
- Remote Monitoring
- Digital Health
---
