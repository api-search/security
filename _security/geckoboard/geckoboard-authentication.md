---
api_key_in: []
api_specs:
- filename: geckoboard-openapi.yml
  format: yaml
  label: Geckoboard Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geckoboard/refs/heads/main/openapi/geckoboard-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Geckoboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geckoboard secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Geckoboard
provider_slug: geckoboard
scheme_count: 1
schemes:
- description: HTTP Basic with the Geckoboard API key as the username and empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/geckoboard-openapi.yml
  type: http
slug: geckoboard-authentication
source_filename: geckoboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/geckoboard-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with the Geckoboard API key as the username and empty password.\n  sources:\n  - openapi/geckoboard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geckoboard/refs/heads/main/authentication/geckoboard-authentication.yml
summary_line: http · 1 scheme
tags:
- Dashboards
- Data Visualization
- Business Intelligence
- KPI Tracking
- Real-Time Reporting
- TV Dashboards
---
