---
api_key_in: []
api_specs:
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman Metrics API
  slug: ultrahuman-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman CGM (Glucose) API
  slug: ultrahuman-cgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman User Info API
  slug: ultrahuman-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman OAuth 2.0 API
  slug: ultrahuman-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ultrahuman Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ultrahuman secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ultrahuman
provider_slug: ultrahuman
scheme_count: 1
schemes:
- description: OAuth 2.0 access token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ultrahuman-openapi.yml
  type: http
slug: ultrahuman-authentication
source_filename: ultrahuman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ultrahuman-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token in the Authorization header.\n  sources:\n  - openapi/ultrahuman-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/authentication/ultrahuman-authentication.yml
summary_line: http · 1 scheme
tags:
- Wearables
- Smart Ring
- Health
- Metabolic Health
- Sleep
- HRV
- Recovery
- CGM
- Glucose
- Digital Health
---
