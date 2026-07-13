---
api_key_in:
- header
api_specs:
- filename: wisk-sales-upload-openapi.yml
  format: yaml
  label: WISK Public Sales Upload API
  slug: sales-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk/refs/heads/main/openapi/wisk-sales-upload-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wisk Authentication
name_suffix: Authentication
oauth_flows: []
overview: WISK.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WISK.ai
provider_slug: wisk
scheme_count: 1
schemes:
- description: Venue unique identifier provisioned by WISK for the partner. The public guide instructs partners to "ask WISK to give the venue unique identifier" and supply it in the request header. The exact header name is assigned by WISK per integration; X-Wisk-Venue-Id is used here as a representative placeholder.
  in: header
  name: venueIdHeader
  parameter: X-Wisk-Venue-Id
  sources:
  - openapi/wisk-sales-upload-openapi.yml
  type: apiKey
slug: wisk-authentication
source_filename: wisk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wisk-sales-upload-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: venueIdHeader\n  type: apiKey\n  in: header\n  parameter: X-Wisk-Venue-Id\n  description: Venue unique identifier provisioned by WISK for the partner. The public guide\n    instructs partners to \"ask WISK to give the venue unique identifier\" and supply it in the\n    request header. The exact header name is assigned by WISK per integration; X-Wisk-Venue-Id\n    is used here as a representative placeholder.\n  sources:\n  - openapi/wisk-sales-upload-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisk/refs/heads/main/authentication/wisk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Bar
- Inventory
- Hospitality
- Sales
- POS Integration
---
