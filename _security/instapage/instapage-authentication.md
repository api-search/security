---
api_key_in: []
api_specs:
- filename: instapage-openapi.yml
  format: yaml
  label: Instapage Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Instapage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instapage secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instapage
provider_slug: instapage
scheme_count: 1
schemes:
- bearerFormat: API key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/instapage-openapi.yml
  type: http
slug: instapage-authentication
source_filename: instapage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instapage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/instapage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/authentication/instapage-authentication.yml
summary_line: http · 1 scheme
tags:
- Landing Pages
- Conversion Optimization
- Marketing
- A/B Testing
- Post-Click Optimization
- Lead Generation
---
