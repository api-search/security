---
api_key_in: []
api_specs:
- filename: maia-analytics-openapi-original.json
  format: json
  label: MAIA API
  slug: maia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maia-analytics/refs/heads/main/openapi/maia-analytics-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maia Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maia-analytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maia-analytics
provider_slug: maia-analytics
scheme_count: 1
schemes:
- name: FirebaseAuthMiddleware
  scheme: bearer
  sources:
  - openapi/maia-analytics-openapi-original.json
  type: http
slug: maia-analytics-authentication
source_filename: maia-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/maia-analytics-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: FirebaseAuthMiddleware\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/maia-analytics-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maia-analytics/refs/heads/main/authentication/maia-analytics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Geospatial
- GIS
- Location Intelligence
- Mapping
- Artificial Intelligence
- Analytics
---
