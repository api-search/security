---
api_key_in:
- header
api_specs:
- filename: checkiday-openapi.yml
  format: yaml
  label: Checkiday Holiday and Event API
  slug: checkiday-holiday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkiday-national-holiday-api/refs/heads/main/openapi/checkiday-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Checkiday National Holiday Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkiday - National Holiday and Event API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkiday - National Holiday and Event API
provider_slug: checkiday-national-holiday-api
scheme_count: 1
schemes:
- description: Your apilayer API key for the Checkiday API. Issued from the apilayer marketplace.
  in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/checkiday-openapi.yml
  type: apiKey
slug: checkiday-national-holiday-api-authentication
source_filename: checkiday-national-holiday-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkiday-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Your apilayer API key for the Checkiday API. Issued from the apilayer marketplace.\n  sources:\n  - openapi/checkiday-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkiday-national-holiday-api/refs/heads/main/authentication/checkiday-national-holiday-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Calendar
- Holidays
- Events
- Observances
- Dates
- Time
- Public APIs
---
