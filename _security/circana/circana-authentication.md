---
api_key_in: []
api_specs:
- filename: circana-liquid-data.yaml
  format: yaml
  label: Circana Liquid Data API
  slug: liquid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-liquid-data.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circana
provider_slug: circana
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained through Circana authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/circana-liquid-data.yaml
  type: http
slug: circana-authentication
source_filename: circana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circana-liquid-data.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained through Circana authentication\n  sources:\n  - openapi/circana-liquid-data.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/authentication/circana-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
---
