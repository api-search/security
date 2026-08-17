---
api_key_in: []
api_specs:
- filename: kissmetrics-products-api-openapi.yml
  format: yaml
  label: Kissmetrics REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kissmetrics/refs/heads/main/openapi/kissmetrics-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kissmetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kissmetrics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kissmetrics
provider_slug: kissmetrics
scheme_count: 1
schemes:
- description: HTTP Basic. Base64 of `username:password` (or of `API_KEY:` with an empty password) in the Authorization header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kissmetrics-exports-api-openapi.yml
  - openapi/kissmetrics-products-api-openapi.yml
  - openapi/kissmetrics-queries-api-openapi.yml
  type: http
slug: kissmetrics-authentication
source_filename: kissmetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/kissmetrics-exports-api-openapi.yml, openapi/kissmetrics-products-api-openapi.yml,\n  openapi/kissmetrics-queries-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic. Base64 of `username:password` (or of `API_KEY:` with an empty password)\n    in the Authorization header.\n  sources:\n  - openapi/kissmetrics-exports-api-openapi.yml\n  - openapi/kissmetrics-products-api-openapi.yml\n  - openapi/kissmetrics-queries-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kissmetrics/refs/heads/main/authentication/kissmetrics-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Product Analytics
- Behavioral Analytics
- Marketing Analytics
- Customer Analytics
- Event Tracking
- Funnels
- Cohorts
- Retention
- Attribution
- Data Export
---
