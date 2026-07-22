---
api_key_in: []
api_specs:
- filename: powernaut-partner-api-openapi-original.yml
  format: yaml
  label: Powernaut Partner API
  slug: powernaut-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-partner-api-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Powernaut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Powernaut secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Powernaut
provider_slug: powernaut
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: A bearer token obtained from the token endpoint.
  name: cloud-cloud
  scheme: bearer
  sources:
  - openapi/powernaut-partner-api-openapi-original.yml
  type: http
- description: Your client id and secret to obtain a bearer token for cloud-cloud authentication.
  name: token
  scheme: basic
  sources:
  - openapi/powernaut-partner-api-openapi-original.yml
  type: http
slug: powernaut-authentication
source_filename: powernaut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/powernaut-partner-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: cloud-cloud\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A bearer token obtained from the token endpoint.\n  sources:\n  - openapi/powernaut-partner-api-openapi-original.yml\n- name: token\n  type: http\n  scheme: basic\n  description: Your client id and secret to obtain a bearer token for cloud-cloud authentication.\n  sources:\n  - openapi/powernaut-partner-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/authentication/powernaut-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Energy
- Virtual Power Plant
- Distributed Energy Resources
- Energy Trading
- Flexibility
- Forecasting
- Grid
---
