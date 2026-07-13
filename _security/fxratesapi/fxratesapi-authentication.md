---
api_key_in: []
api_specs:
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Latest Rates API
  slug: fxratesapi-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Historical Rates API
  slug: fxratesapi-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Time-Series API
  slug: fxratesapi-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Convert API
  slug: fxratesapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Currencies API
  slug: fxratesapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: probed
name: Fxratesapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: FXRatesAPI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FXRatesAPI
provider_slug: fxratesapi
scheme_count: 2
schemes:
- description: API key passed as the api_key query parameter, e.g. https://api.fxratesapi.com/latest?api_key=YOUR_KEY. Confirmed accepted (HTTP 200) during live probing.
  in: query
  keyName: api_key
  name: apiKeyQuery
  sources:
  - https://fxratesapi.com/docs/authentication
  - openapi/fxratesapi-openapi.yml
  type: apiKey
- description: 'API key passed as an Authorization: Bearer YOUR_KEY header, per the FXRatesAPI authentication documentation.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://fxratesapi.com/docs/authentication
  - openapi/fxratesapi-openapi.yml
  type: http
slug: fxratesapi-authentication
source_filename: fxratesapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live probes of api.fxratesapi.com + fxratesapi.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  keyName: api_key\n  description: >-\n    API key passed as the api_key query parameter, e.g.\n    https://api.fxratesapi.com/latest?api_key=YOUR_KEY. Confirmed accepted\n    (HTTP 200) during live probing.\n  sources:\n  - https://fxratesapi.com/docs/authentication\n  - openapi/fxratesapi-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key passed as an Authorization: Bearer YOUR_KEY header, per the\n    FXRatesAPI authentication documentation.\n  sources:\n  - https://fxratesapi.com/docs/authentication\n  - openapi/fxratesapi-openapi.yml\naccessModel:\n  anonymousTier: true\n  notes: >-\n    A limited tier is usable without any API key. GET /latest, /historical,\n    /timeseries, /convert, and /currencies all\
  \ returned HTTP 200 with valid JSON\n    when called anonymously on 2026-07-12, and an obviously invalid api_key value\n    was ignored (the request still succeeded as anonymous) rather than rejected.\n    A paid API key raises request quotas, increases update frequency, and unlocks\n    base-currency switching per the pricing page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/authentication/fxratesapi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Foreign Exchange
- FX
- Currency
- Exchange Rates
- Forex
- Currency Conversion
- Historical Rates
- Financial Data
- Cryptocurrencies
---
