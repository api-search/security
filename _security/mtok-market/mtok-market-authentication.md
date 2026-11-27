---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mtok-market-agents-api-openapi.yml
  format: yaml
  label: mtok.market Agents API
  slug: mtok-market-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-agents-api-openapi.yml
- filename: mtok-market-bids-api-openapi.yml
  format: yaml
  label: mtok.market Bids API
  slug: mtok-market-bids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-bids-api-openapi.yml
- filename: mtok-market-book-api-openapi.yml
  format: yaml
  label: mtok.market Book API
  slug: mtok-market-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-book-api-openapi.yml
- filename: mtok-market-chain-api-openapi.yml
  format: yaml
  label: mtok.market Chain API
  slug: mtok-market-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-chain-api-openapi.yml
- filename: mtok-market-config-api-openapi.yml
  format: yaml
  label: mtok.market Config API
  slug: mtok-market-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-config-api-openapi.yml
- filename: mtok-market-exchange-api-openapi.yml
  format: yaml
  label: mtok.market Exchange API
  slug: mtok-market-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-exchange-api-openapi.yml
- filename: mtok-market-feedback-api-openapi.yml
  format: yaml
  label: mtok.market Feedback API
  slug: mtok-market-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-feedback-api-openapi.yml
- filename: mtok-market-guides-api-openapi.yml
  format: yaml
  label: mtok.market Guides API
  slug: mtok-market-guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-guides-api-openapi.yml
- filename: mtok-market-health-api-openapi.yml
  format: yaml
  label: mtok.market Health API
  slug: mtok-market-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-health-api-openapi.yml
- filename: mtok-market-mcp-api-openapi.yml
  format: yaml
  label: mtok.market MCP API
  slug: mtok-market-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-mcp-api-openapi.yml
- filename: mtok-market-me-api-openapi.yml
  format: yaml
  label: mtok.market Me API
  slug: mtok-market-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-me-api-openapi.yml
- filename: mtok-market-models-api-openapi.yml
  format: yaml
  label: mtok.market Models API
  slug: mtok-market-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-models-api-openapi.yml
- filename: mtok-market-offers-api-openapi.yml
  format: yaml
  label: mtok.market Offers API
  slug: mtok-market-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-offers-api-openapi.yml
- filename: mtok-market-orderlog-api-openapi.yml
  format: yaml
  label: mtok.market Orderlog API
  slug: mtok-market-orderlog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-orderlog-api-openapi.yml
- filename: mtok-market-spot-api-openapi.yml
  format: yaml
  label: mtok.market Spot API
  slug: mtok-market-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtok-market/openapi/mtok-market-spot-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: mtok.market Authentication
name_suffix: Authentication
oauth_flows: []
overview: mtok.market secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mtok.market
provider_slug: mtok-market
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/mtok-market-openapi.json
  type: apiKey
slug: mtok-market-authentication
source_filename: mtok-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mtok-market-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/mtok-market-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mtok-market/authentication/mtok-market-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Tokens
- Non-Custodial
- Spot Pricing
---
