---
api_key_in: []
api_specs:
- filename: metronome-openapi.json
  format: json
  label: Metronome API
  slug: metronome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Metronome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metronome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metronome
provider_slug: metronome
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/metronome-openapi.json
  type: http
slug: metronome-authentication
source_filename: metronome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metronome-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/metronome-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/authentication/metronome-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- FinOps
- Metering
- Pricing
- Usage-Based Billing
---
