---
api_key_in: []
api_specs:
- filename: pinnacle-openapi.yml
  format: yaml
  label: Pinnacle Customer API
  slug: pinnacle-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/openapi/pinnacle-openapi.yml
- filename: pinnacle-asyncapi.yml
  format: yaml
  label: Pinnacle Lines API
  slug: pinnacle-lines-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/openapi/pinnacle-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinnacle Authentication
name_suffix: Authentication
oauth_flows: []
overview: ' Pinnacle Sports Betting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.'
provider_name: ' Pinnacle Sports Betting'
provider_slug: pinnacle-sports-betting
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/pinnacle-openapi.yml
  type: http
slug: pinnacle-authentication
source_filename: pinnacle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinnacle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/pinnacle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/authentication/pinnacle-authentication.yml
summary_line: http · 1 scheme
tags:
- Gambling
- Sports Betting
---
