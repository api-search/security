---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: unirateapi-commodity-api-openapi.yml
  format: yaml
  label: UniRate API Commodity API
  slug: unirateapi-commodity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-commodity-api-openapi.yml
- filename: unirateapi-currency-api-openapi.yml
  format: yaml
  label: UniRate API Currency API
  slug: unirateapi-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-currency-api-openapi.yml
- filename: unirateapi-historical-currency-api-openapi.yml
  format: yaml
  label: UniRate API Historical Currency API
  slug: unirateapi-historical-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-historical-currency-api-openapi.yml
- filename: unirateapi-vat-rates-api-openapi.yml
  format: yaml
  label: UniRate API VAT Rates API
  slug: unirateapi-vat-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/openapi/unirateapi-vat-rates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Unirateapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: UniRate API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UniRate API
provider_slug: unirateapi
scheme_count: 1
schemes:
- description: Your UniRate API key, passed as the `api_key` query parameter.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/unirateapi-openapi.yaml
  type: apiKey
slug: unirateapi-authentication
source_filename: unirateapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: derived\nsource: openapi/unirateapi-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Your UniRate API key, passed as the `api_key` query parameter.\n  sources:\n  - openapi/unirateapi-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unirateapi/refs/heads/main/authentication/unirateapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency
- Exchange Rates
- Foreign Exchange
- Forex
- Currency Conversion
- VAT
- Finance
- Financial Data
---
