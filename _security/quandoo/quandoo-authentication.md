---
api_key_in:
- header
api_specs:
- filename: quandoo-public-partner-api-openapi.yml
  format: yaml
  label: Quandoo Public Partner API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-public-partner-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quandoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quandoo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quandoo
provider_slug: quandoo
scheme_count: 1
schemes:
- in: header
  name: API_TOKEN
  parameter: X-Quandoo-AuthToken
  sources:
  - openapi/quandoo-public-partner-api-openapi.yml
  type: apiKey
slug: quandoo-authentication
source_filename: quandoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quandoo-public-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_TOKEN\n  type: apiKey\n  in: header\n  parameter: X-Quandoo-AuthToken\n  sources:\n  - openapi/quandoo-public-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/authentication/quandoo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Reservations
- Booking
- Availability
- Merchants
- Marketplace
---
