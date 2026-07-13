---
api_key_in:
- header
- query
api_specs:
- filename: currencylayer-openapi.yml
  format: yaml
  label: Currencylayer API
  slug: currencylayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/openapi/currencylayer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Currencylayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Currencylayer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Currencylayer
provider_slug: currencylayer
scheme_count: 2
schemes:
- description: APILayer marketplace API key (https://apilayer.com/marketplace/currency_data-api).
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/currencylayer-openapi.yml
  type: apiKey
- description: Legacy Currencylayer access key (https://currencylayer.com/dashboard).
  in: query
  name: AccessKeyQuery
  parameter: access_key
  sources:
  - openapi/currencylayer-openapi.yml
  type: apiKey
slug: currencylayer-authentication
source_filename: currencylayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/currencylayer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: APILayer marketplace API key (https://apilayer.com/marketplace/currency_data-api).\n  sources:\n  - openapi/currencylayer-openapi.yml\n- name: AccessKeyQuery\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: Legacy Currencylayer access key (https://currencylayer.com/dashboard).\n  sources:\n  - openapi/currencylayer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/authentication/currencylayer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Forex
- Conversion
- Historical Rates
- Time Frame
- Change Report
- Precious Metals
- APILayer
- Public APIs
---
