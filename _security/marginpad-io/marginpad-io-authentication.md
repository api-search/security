---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: marginpad-io-calculators-api-openapi.yml
  format: yaml
  label: MarginPad Calculators API
  slug: marginpad-io-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-calculators-api-openapi.yml
- filename: marginpad-io-derivatives-api-openapi.yml
  format: yaml
  label: MarginPad Derivatives API
  slug: marginpad-io-derivatives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-derivatives-api-openapi.yml
- filename: marginpad-io-macro-api-openapi.yml
  format: yaml
  label: MarginPad Macro API
  slug: marginpad-io-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-macro-api-openapi.yml
- filename: marginpad-io-market-data-api-openapi.yml
  format: yaml
  label: MarginPad Market data API
  slug: marginpad-io-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-market-data-api-openapi.yml
- filename: marginpad-io-meta-api-openapi.yml
  format: yaml
  label: MarginPad Meta API
  slug: marginpad-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-meta-api-openapi.yml
- filename: marginpad-io-order-book-api-openapi.yml
  format: yaml
  label: MarginPad Order book API
  slug: marginpad-io-order-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-order-book-api-openapi.yml
- filename: marginpad-io-paper-trading-api-openapi.yml
  format: yaml
  label: MarginPad Paper trading API
  slug: marginpad-io-paper-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-paper-trading-api-openapi.yml
- filename: marginpad-io-plans-api-openapi.yml
  format: yaml
  label: MarginPad Plans API
  slug: marginpad-io-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-plans-api-openapi.yml
- filename: marginpad-io-regional-quotes-api-openapi.yml
  format: yaml
  label: MarginPad Regional quotes API
  slug: marginpad-io-regional-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-regional-quotes-api-openapi.yml
- filename: marginpad-io-screener-api-openapi.yml
  format: yaml
  label: MarginPad Screener API
  slug: marginpad-io-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marginpad-io/openapi/marginpad-io-screener-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MarginPad Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarginPad secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarginPad
provider_slug: marginpad-io
scheme_count: 1
schemes:
- description: Required for paper-trading endpoints; OPTIONAL on /api/v1/* data endpoints, where sending it moves the call from the 60/minute per-IP limit to the key’s own budget (120/minute on Free, 600 on API Pro, 2000 on Max, 5000 on Business). Mint a key at POST /api/bot/key while signed in, or on https://marginpad.io/trading-api/.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/marginpad-io-openapi.json
  type: apiKey
slug: marginpad-io-authentication
source_filename: marginpad-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/marginpad-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Required for paper-trading endpoints; OPTIONAL on /api/v1/* data endpoints, where\n    sending it moves the call from the 60/minute per-IP limit to the key’s own budget (120/minute\n    on Free, 600 on API Pro, 2000 on Max, 5000 on Business). Mint a key at POST /api/bot/key\n    while signed in, or on https://marginpad.io/trading-api/.\n  sources:\n  - openapi/marginpad-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/marginpad-io/authentication/marginpad-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Trading
- Education
- Paper Trading
---
