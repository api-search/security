---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asrai-me-ai-api-openapi.yml
  format: yaml
  label: Asrai AI API
  slug: asrai-me-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-ai-api-openapi.yml
- filename: asrai-me-cashflow-api-openapi.yml
  format: yaml
  label: Asrai Cashflow API
  slug: asrai-me-cashflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-cashflow-api-openapi.yml
- filename: asrai-me-market-data-api-openapi.yml
  format: yaml
  label: Asrai Market Data API
  slug: asrai-me-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-market-data-api-openapi.yml
- filename: asrai-me-screeners-api-openapi.yml
  format: yaml
  label: Asrai Screeners API
  slug: asrai-me-screeners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-screeners-api-openapi.yml
- filename: asrai-me-technical-api-openapi.yml
  format: yaml
  label: Asrai Technical API
  slug: asrai-me-technical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-technical-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Asrai Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Asrai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Asrai
provider_slug: asrai-me
scheme_count: 2
schemes:
- description: 'Bearer token auth – set Authorization: Bearer 0x<private_key>'
  scheme: bearer
  type: http
- description: Native x402 protocol – requires x402-compatible HTTP client
  name: x402
  type: custom
slug: asrai-me-authentication
source_filename: asrai-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: \"openapi/asrai-me-openapi.yml\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Bearer token auth – set Authorization: Bearer 0x<private_key>\"\n  - type: custom\n    name: x402\n    description: \"Native x402 protocol – requires x402-compatible HTTP client\"\n"
source_yaml_url: https://artifacts.apis.io/asrai-me/authentication/asrai-me-authentication.yml
summary_line: 2 schemes
tags:
- Cryptocurrency
- Artificial Intelligence
- Trading
- Signals
- Telegram
- Analytics
---
