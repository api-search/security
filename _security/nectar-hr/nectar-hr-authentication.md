---
api_key_in: []
api_specs:
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Users API
  slug: nectar-hr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Recognition API
  slug: nectar-hr-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Custom Awards API
  slug: nectar-hr-custom-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Financial Analytics API
  slug: nectar-hr-financial-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Flows API
  slug: nectar-hr-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nectar Hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nectar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nectar
provider_slug: nectar-hr
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nectar-hr-openapi.yml
  type: http
slug: nectar-hr-authentication
source_filename: nectar-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nectar-hr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nectar-hr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/authentication/nectar-hr-authentication.yml
summary_line: http · 1 scheme
tags:
- Employee Recognition
- Rewards
- Points
- HR
- Employee Engagement
- Culture
- People Operations
---
