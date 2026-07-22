---
api_key_in:
- header
api_specs:
- filename: synthego-order-openapi.json
  format: json
  label: Synthego Order API
  slug: synthego-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthego/refs/heads/main/openapi/synthego-order-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Synthego Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthego secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synthego
provider_slug: synthego
scheme_count: 1
schemes:
- in: header
  name: UserSecurity
  parameter: SYNTHEGOAPIKEY
  sources:
  - openapi/synthego-order-openapi.json
  type: apiKey
slug: synthego-authentication
source_filename: synthego-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/synthego-order-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: UserSecurity\n  type: apiKey\n  in: header\n  parameter: SYNTHEGOAPIKEY\n  sources:\n  - openapi/synthego-order-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthego/refs/heads/main/authentication/synthego-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health Tech
- Genomics
- CRISPR
- Biotechnology
- Life Sciences
- Synthetic Biology
- Ordering
---
