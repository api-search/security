---
api_key_in:
- header
api_specs:
- filename: fixer-conversion-api-openapi.yml
  format: yaml
  label: Fixer Conversion API
  slug: fixer-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-conversion-api-openapi.yml
- filename: fixer-fluctuation-api-openapi.yml
  format: yaml
  label: Fixer Fluctuation API
  slug: fixer-fluctuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-fluctuation-api-openapi.yml
- filename: fixer-rates-api-openapi.yml
  format: yaml
  label: Fixer Rates API
  slug: fixer-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-rates-api-openapi.yml
- filename: fixer-symbols-api-openapi.yml
  format: yaml
  label: Fixer Symbols API
  slug: fixer-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-symbols-api-openapi.yml
- filename: fixer-time-series-api-openapi.yml
  format: yaml
  label: Fixer Time Series API
  slug: fixer-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-time-series-api-openapi.yml
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
