---
api_key_in:
- header
api_specs:
- filename: united-rentals-total-control-openapi.yml
  format: yaml
  label: United Rentals Total Control Integration API
  slug: united-rentals-total-control-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-rentals/main/openapi/united-rentals-total-control-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: United Rentals Authentication
name_suffix: Authentication
oauth_flows: []
overview: United Rentals secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United Rentals
provider_slug: united-rentals
scheme_count: 1
schemes:
- description: United Rentals API key from Total Control portal
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/united-rentals-total-control-openapi.yml
  type: apiKey
slug: united-rentals-authentication
source_filename: united-rentals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-rentals-total-control-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: United Rentals API key from Total Control portal\n  sources:\n  - openapi/united-rentals-total-control-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-rentals/refs/heads/main/authentication/united-rentals-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Equipment Rental
- Procurement
- Supply Chain
- Construction
- Fortune 500
---
