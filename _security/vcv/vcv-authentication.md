---
api_key_in: []
api_specs:
- filename: vcv-openapi.yml
  format: yaml
  label: VCV Open API
  slug: vcv-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vcv Authentication
name_suffix: Authentication
oauth_flows: []
overview: VCV secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VCV
provider_slug: vcv
scheme_count: 1
schemes:
- bearerFormat: token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vcv-openapi-original.yml
  - openapi/vcv-openapi.yml
  type: http
slug: vcv-authentication
source_filename: vcv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vcv-openapi-original.yml, openapi/vcv-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/vcv-openapi-original.yml\n  - openapi/vcv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/authentication/vcv-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Recruiting
- Human Resources
- Video Interviews
- Talent Acquisition
- Hiring
- Assessments
---
