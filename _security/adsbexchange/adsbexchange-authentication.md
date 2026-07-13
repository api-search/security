---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: ADS-B Exchange Aircraft API
  slug: ads-b-exchange-aircraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Adsbexchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADS-B Exchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ADS-B Exchange
provider_slug: adsbexchange
scheme_count: 1
schemes:
- description: Provide your API key via x-api-key header to access the API.
  in: header
  name: X-Api-Key
  parameter: x-api-key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: adsbexchange-authentication
source_filename: adsbexchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Provide your API key via x-api-key header to access the API.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/authentication/adsbexchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Real-Time
- Military
- MLAT
---
