---
api_key_in:
- query
api_specs:
- filename: open-exchange-rates-convert-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Convert API
  slug: open-exchange-rates-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-convert-api-openapi.yml
- filename: open-exchange-rates-currencies-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Currencies API
  slug: open-exchange-rates-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-currencies-api-openapi.yml
- filename: open-exchange-rates-ohlc-api-openapi.yml
  format: yaml
  label: Open Exchange Rates OHLC API
  slug: open-exchange-rates-ohlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-ohlc-api-openapi.yml
- filename: open-exchange-rates-rates-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Rates API
  slug: open-exchange-rates-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-rates-api-openapi.yml
- filename: open-exchange-rates-time-series-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Time Series API
  slug: open-exchange-rates-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-time-series-api-openapi.yml
- filename: open-exchange-rates-usage-api-openapi.yml
  format: yaml
  label: Open Exchange Rates Usage API
  slug: open-exchange-rates-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/openapi/open-exchange-rates-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Open Exchange Rates Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Exchange Rates secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Exchange Rates
provider_slug: open-exchange-rates
scheme_count: 1
schemes:
- description: Your unique App ID obtained from openexchangerates.org. Required for all endpoints except /currencies.json.
  in: query
  name: appId
  parameter: app_id
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: open-exchange-rates-authentication
source_filename: open-exchange-rates-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: appId\n  type: apiKey\n  in: query\n  parameter: app_id\n  description: Your unique App ID obtained from openexchangerates.org. Required for all endpoints\n    except /currencies.json.\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-exchange-rates/refs/heads/main/authentication/open-exchange-rates-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Foreign Exchange
- Currency
- Forex
- Finance
- Exchange Rates
- Currency Conversion
- Historical Rates
---
