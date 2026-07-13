---
api_key_in: []
api_specs:
- filename: aspentech-inmation-web-openapi.yml
  format: yaml
  label: AspenTech Inmation Web API
  slug: inmation-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-inmation-web-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aspentech Authentication
name_suffix: Authentication
oauth_flows: []
overview: AspenTech secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AspenTech
provider_slug: aspentech
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/aspentech-inmation-web-openapi.yml
  type: http
- name: bearerToken
  scheme: bearer
  sources:
  - openapi/aspentech-inmation-web-openapi.yml
  type: http
slug: aspentech-authentication
source_filename: aspentech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aspentech-inmation-web-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/aspentech-inmation-web-openapi.yml\n- name: bearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aspentech-inmation-web-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/authentication/aspentech-authentication.yml
summary_line: http · 2 schemes
tags:
- Industrial IoT
- Process Optimization
- Manufacturing
- Energy
- Chemicals
- Time Series
---
