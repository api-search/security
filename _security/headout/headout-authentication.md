---
api_key_in:
- header
api_specs:
- filename: headout-partner-openapi.yml
  format: yaml
  label: Headout Partner API
  slug: headout-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/headout/refs/heads/main/openapi/headout-partner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Headout Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeadOut secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HeadOut
provider_slug: headout
scheme_count: 1
schemes:
- description: API token. Production keys are prefixed pk_, testing keys tk_.
  in: header
  name: HeadoutAuth
  parameter: Headout-Auth
  sources:
  - openapi/headout-partner-openapi.yml
  type: apiKey
slug: headout-authentication
source_filename: headout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/headout-partner-openapi.yml\ndocs: https://github.com/headout/api-docs/blob/master/conventions/basics.md\nnotes: >-\n  All Partner APIs authenticate with the Headout-Auth request header carrying an\n  API token. Production tokens are prefixed pk_ (live bookings), testing tokens\n  tk_ (sandbox). V2 requires auth on every call; some V1 read endpoints (e.g.\n  inventory) are optional but auth is recommended. Keys are issued by email via\n  partnerships@headout.com / apikey@headout.com. No OAuth surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HeadoutAuth\n  type: apiKey\n  in: header\n  parameter: Headout-Auth\n  description: API token. Production keys are prefixed pk_, testing keys tk_.\n  sources:\n  - openapi/headout-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headout/refs/heads/main/authentication/headout-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel
- Tours and Activities
- Experiences
- Attractions
- Ticketing
- Bookings
- Marketplace
- Partner API
- Affiliate
- Events
---
