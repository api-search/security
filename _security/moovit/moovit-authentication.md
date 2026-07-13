---
api_key_in:
- header
api_specs:
- filename: moovit-public-transit-api-openapi.yml
  format: yaml
  label: Moovit Public Transit API
  slug: moovit-public-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-public-transit-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Moovit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moovit secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moovit
provider_slug: moovit
scheme_count: 2
schemes:
- description: HMAC-SHA256 signature in the form `hmacauth <signature>:<nonce>:<timestamp>` over `<timestamp>:<payload>:<nonce>` using the API secret key.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/moovit-public-transit-api-openapi.yml
  type: apiKey
- description: Public API key issued by Moovit. Required on every request.
  in: header
  name: apiKey
  parameter: API_KEY
  sources:
  - openapi/moovit-public-transit-api-openapi.yml
  type: apiKey
slug: moovit-authentication
source_filename: moovit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moovit-public-transit-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 signature in the form `hmacauth <signature>:<nonce>:<timestamp>`\n    over `<timestamp>:<payload>:<nonce>` using the API secret key.\n  sources:\n  - openapi/moovit-public-transit-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: API_KEY\n  description: Public API key issued by Moovit. Required on every request.\n  sources:\n  - openapi/moovit-public-transit-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/authentication/moovit-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Transit
- Public Transit
- Mobility
- Mobility As A Service
- MaaS
- Trip Planning
- Multimodal Routing
- Real Time
- GTFS
- GTFS Realtime
- Service Alerts
- Smart Cities
- Transportation
- Mobileye
- Intel
---
