---
api_key_in:
- header
api_specs:
- filename: dhl-openapi.yml
  format: yaml
  label: Location Finder Unified
  slug: location-finder-unified
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dhl/refs/heads/main/openapi/dhl-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dhl Authentication
name_suffix: Authentication
oauth_flows: []
overview: DHL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DHL
provider_slug: dhl
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: DHL-API-Key
  sources:
  - openapi/dhl-openapi.yml
  type: apiKey
slug: dhl-authentication
source_filename: dhl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dhl-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: DHL-API-Key\n  sources:\n  - openapi/dhl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dhl/refs/heads/main/authentication/dhl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Freight
- Logistics
- Shipping
- eCommerce
- Tracking
---
