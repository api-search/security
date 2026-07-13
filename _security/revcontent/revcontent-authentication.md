---
api_key_in: []
api_specs:
- filename: revcontent-stats-management-openapi.yml
  format: yaml
  label: RevContent Stats & Management API
  slug: revcontent-stats-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-stats-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Revcontent Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevContent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RevContent
provider_slug: revcontent
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from /oauth/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/revcontent-stats-management-openapi.yml
  type: http
slug: revcontent-authentication
source_filename: revcontent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revcontent-stats-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from /oauth/token\n  sources:\n  - openapi/revcontent-stats-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/authentication/revcontent-authentication.yml
summary_line: http · 1 scheme
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
---
