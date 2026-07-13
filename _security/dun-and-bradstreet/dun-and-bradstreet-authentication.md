---
api_key_in: []
api_specs:
- filename: dnb-direct-plus-openapi-original.yml
  format: yaml
  label: D&B Direct+ API
  slug: direct-plus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dnb-direct-plus-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dun And Bradstreet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dun & Bradstreet secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dun & Bradstreet
provider_slug: dun-and-bradstreet
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dnb-direct-plus-openapi-original.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/dnb-direct-plus-openapi-original.yml
  type: http
slug: dun-and-bradstreet-authentication
source_filename: dun-and-bradstreet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dnb-direct-plus-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dnb-direct-plus-openapi-original.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dnb-direct-plus-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/authentication/dun-and-bradstreet-authentication.yml
summary_line: http · 2 schemes
tags:
- Business Data
- Company Data
- D-U-N-S Number
- Credit
- Risk
- Master Data
- Data Enrichment
- Identity Resolution
- Compliance
- Supply Chain
- Sales Intelligence
- Monitoring
---
