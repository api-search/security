---
api_key_in:
- header
api_specs:
- filename: fixer-openapi.yml
  format: yaml
  label: Fixer API
  slug: fixer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fixer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fixer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fixer
provider_slug: fixer
scheme_count: 1
schemes:
- description: APILayer API key provisioned at https://apilayer.com/marketplace/fixer-api.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/fixer-openapi.yml
  type: apiKey
slug: fixer-authentication
source_filename: fixer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fixer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: APILayer API key provisioned at https://apilayer.com/marketplace/fixer-api.\n  sources:\n  - openapi/fixer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/authentication/fixer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Forex
- ECB
- Conversion
- Historical Rates
- Time Series
- Fluctuation
- APILayer
- Public APIs
---
