---
api_key_in: []
api_specs:
- filename: leapsome-content-api-openapi.yml
  format: yaml
  label: Leapsome Content API
  slug: leapsome-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-content-api-openapi.yml
- filename: leapsome-scim-api-openapi.yml
  format: yaml
  label: Leapsome SCIM API
  slug: leapsome-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-scim-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leapsome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leapsome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leapsome
provider_slug: leapsome
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leapsome-content-api-openapi.yml
  - openapi/leapsome-scim-api-openapi.yml
  type: http
slug: leapsome-authentication
source_filename: leapsome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leapsome-content-api-openapi.yml, openapi/leapsome-scim-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/leapsome-content-api-openapi.yml\n  - openapi/leapsome-scim-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/authentication/leapsome-authentication.yml
summary_line: http · 1 scheme
tags:
- People Enablement
- Performance Management
- OKRs
- Goals
- Engagement Surveys
- HRIS
- SCIM
- Employee Development
- 1:1 Meetings
- Learning
---
