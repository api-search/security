---
api_key_in:
- header
api_specs:
- filename: bjs-wholesale-club-openapi.yaml
  format: yaml
  label: BJ's Wholesale Club API
  slug: bjs-wholesale-club
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/openapi/bjs-wholesale-club-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bjs Wholesale Club Authentication
name_suffix: Authentication
oauth_flows: []
overview: BJ's Wholesale Club secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-BJS-API-Key
  sources:
  - openapi/bjs-wholesale-club-openapi.yaml
  type: apiKey
slug: bjs-wholesale-club-authentication
source_filename: bjs-wholesale-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bjs-wholesale-club-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-BJS-API-Key\n  sources:\n  - openapi/bjs-wholesale-club-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/authentication/bjs-wholesale-club-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
---
