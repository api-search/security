---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dripmetrics-ai-aerodrome-api-openapi.yml
  format: yaml
  label: DripMetrics AI Aerodrome API
  slug: dripmetrics-ai-aerodrome-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-aerodrome-api-openapi.yml
- filename: dripmetrics-ai-btc-options-api-openapi.yml
  format: yaml
  label: DripMetrics AI BTC options API
  slug: dripmetrics-ai-btc-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-btc-options-api-openapi.yml
- filename: dripmetrics-ai-discovery-api-openapi.yml
  format: yaml
  label: DripMetrics AI Discovery API
  slug: dripmetrics-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-discovery-api-openapi.yml
- filename: dripmetrics-ai-exchange-metrics-api-openapi.yml
  format: yaml
  label: DripMetrics AI Exchange metrics API
  slug: dripmetrics-ai-exchange-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-exchange-metrics-api-openapi.yml
- filename: dripmetrics-ai-hyperliquid-api-openapi.yml
  format: yaml
  label: DripMetrics AI Hyperliquid API
  slug: dripmetrics-ai-hyperliquid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-hyperliquid-api-openapi.yml
- filename: dripmetrics-ai-hyperliquid-book-api-openapi.yml
  format: yaml
  label: DripMetrics AI Hyperliquid book API
  slug: dripmetrics-ai-hyperliquid-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-hyperliquid-book-api-openapi.yml
- filename: dripmetrics-ai-kraken-xstocks-api-openapi.yml
  format: yaml
  label: DripMetrics AI Kraken xStocks API
  slug: dripmetrics-ai-kraken-xstocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-kraken-xstocks-api-openapi.yml
- filename: dripmetrics-ai-market-summary-api-openapi.yml
  format: yaml
  label: DripMetrics AI Market summary API
  slug: dripmetrics-ai-market-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-market-summary-api-openapi.yml
- filename: dripmetrics-ai-on-chain-api-openapi.yml
  format: yaml
  label: DripMetrics AI On Chain API
  slug: dripmetrics-ai-on-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-on-chain-api-openapi.yml
- filename: dripmetrics-ai-orderbook-api-openapi.yml
  format: yaml
  label: DripMetrics AI Orderbook API
  slug: dripmetrics-ai-orderbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-orderbook-api-openapi.yml
- filename: dripmetrics-ai-polymarket-api-openapi.yml
  format: yaml
  label: DripMetrics AI Polymarket API
  slug: dripmetrics-ai-polymarket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-polymarket-api-openapi.yml
- filename: dripmetrics-ai-portfolio-risk-api-openapi.yml
  format: yaml
  label: DripMetrics AI Portfolio risk API
  slug: dripmetrics-ai-portfolio-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-portfolio-risk-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DripMetrics AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: DripMetrics AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DripMetrics AI
provider_slug: dripmetrics-ai
scheme_count: 1
schemes:
- description: x402 v2 payment signature header supplied after reading the 402 PAYMENT-REQUIRED response.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/dripmetrics-ai-openapi.json
  type: apiKey
slug: dripmetrics-ai-authentication
source_filename: dripmetrics-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dripmetrics-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 payment signature header supplied after reading the 402 PAYMENT-REQUIRED\n    response.\n  sources:\n  - openapi/dripmetrics-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dripmetrics-ai/authentication/dripmetrics-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Market Data
- Analytics
- Artificial Intelligence
- Cryptocurrency
---
