---
api_key_in:
- header
api_specs:
- filename: amc-theatres-api-openapi.yml
  format: yaml
  label: AMC Theatres API
  slug: amc-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-theatres-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amc Entertainment Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMC Entertainment Holdings secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AMC Entertainment Holdings
provider_slug: amc-entertainment-holdings
scheme_count: 1
schemes:
- description: AMC vendor API key issued via the AMC Theatres developer portal.
  in: header
  name: VendorKey
  parameter: X-AMC-Vendor-Key
  sources:
  - openapi/amc-theatres-api-openapi.yml
  type: apiKey
slug: amc-entertainment-holdings-authentication
source_filename: amc-entertainment-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amc-theatres-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VendorKey\n  type: apiKey\n  in: header\n  parameter: X-AMC-Vendor-Key\n  description: AMC vendor API key issued via the AMC Theatres developer portal.\n  sources:\n  - openapi/amc-theatres-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/authentication/amc-entertainment-holdings-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entertainment
- Movies
- Theatres
- Showtimes
- Ticketing
- Concessions
- Loyalty
- Fortune 500
---
