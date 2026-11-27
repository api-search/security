---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commodities-sh-calendar-api-openapi.yml
  format: yaml
  label: commodities.sh Calendar API
  slug: commodities-sh-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-calendar-api-openapi.yml
- filename: commodities-sh-catalog-api-openapi.yml
  format: yaml
  label: commodities.sh Catalog API
  slug: commodities-sh-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-catalog-api-openapi.yml
- filename: commodities-sh-cot-api-openapi.yml
  format: yaml
  label: commodities.sh Cot API
  slug: commodities-sh-cot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-cot-api-openapi.yml
- filename: commodities-sh-curve-api-openapi.yml
  format: yaml
  label: commodities.sh Curve API
  slug: commodities-sh-curve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-curve-api-openapi.yml
- filename: commodities-sh-decision-api-openapi.yml
  format: yaml
  label: commodities.sh Decision API
  slug: commodities-sh-decision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-decision-api-openapi.yml
- filename: commodities-sh-fundamentals-api-openapi.yml
  format: yaml
  label: commodities.sh Fundamentals API
  slug: commodities-sh-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-fundamentals-api-openapi.yml
- filename: commodities-sh-fx-api-openapi.yml
  format: yaml
  label: commodities.sh Fx API
  slug: commodities-sh-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-fx-api-openapi.yml
- filename: commodities-sh-health-api-openapi.yml
  format: yaml
  label: commodities.sh Health API
  slug: commodities-sh-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-health-api-openapi.yml
- filename: commodities-sh-history-api-openapi.yml
  format: yaml
  label: commodities.sh History API
  slug: commodities-sh-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-history-api-openapi.yml
- filename: commodities-sh-inventory-api-openapi.yml
  format: yaml
  label: commodities.sh Inventory API
  slug: commodities-sh-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-inventory-api-openapi.yml
- filename: commodities-sh-llms-full-txt-api-openapi.yml
  format: yaml
  label: commodities.sh Llms Full.txt API
  slug: commodities-sh-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-llms-full-txt-api-openapi.yml
- filename: commodities-sh-llms-txt-api-openapi.yml
  format: yaml
  label: commodities.sh Llms.txt API
  slug: commodities-sh-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-llms-txt-api-openapi.yml
- filename: commodities-sh-mcp-api-openapi.yml
  format: yaml
  label: commodities.sh MCP API
  slug: commodities-sh-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-mcp-api-openapi.yml
- filename: commodities-sh-price-api-openapi.yml
  format: yaml
  label: commodities.sh Price API
  slug: commodities-sh-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-price-api-openapi.yml
- filename: commodities-sh-prices-api-openapi.yml
  format: yaml
  label: commodities.sh Prices API
  slug: commodities-sh-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-prices-api-openapi.yml
- filename: commodities-sh-skill-md-api-openapi.yml
  format: yaml
  label: commodities.sh SKILL.md API
  slug: commodities-sh-skill-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-skill-md-api-openapi.yml
- filename: commodities-sh-snapshot-api-openapi.yml
  format: yaml
  label: commodities.sh Snapshot API
  slug: commodities-sh-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-snapshot-api-openapi.yml
- filename: commodities-sh-spreads-api-openapi.yml
  format: yaml
  label: commodities.sh Spreads API
  slug: commodities-sh-spreads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-spreads-api-openapi.yml
- filename: commodities-sh-well-known-api-openapi.yml
  format: yaml
  label: commodities.sh .well Known API
  slug: commodities-sh-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commodities-sh/openapi/commodities-sh-well-known-api-openapi.yml
auth_types:
- x402
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: commodities.sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: commodities.sh secures its APIs with x402 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: commodities.sh
provider_slug: commodities-sh
scheme_count: 2
schemes:
- asset: USDC
  description: 'Agents should use x402: probe a paid route, settle USDC on Base from the 402 challenge, retry with X-PAYMENT. No long-lived secret is required.'
  header: X-PAYMENT
  name: x402
  network: eip155:8453
  scheme: x402 (HTTP 402 Payment Required, USDC on Base)
  sources:
  - https://commodities.sh/docs/authentication
  - https://commodities.sh/x402
  type: x402
- description: 'Human operators buy Pro ($19/mo or $180/yr) at /get-started, receive a cs_live_… key once, and send Authorization: Bearer cs_live_… on paid routes. Each call debits credits (1 credit = $0.01 of list price). Exhausted quota returns HTTP 402 QUOTA_EXCEEDED.'
  key_prefix: cs_live_
  name: ProApiKey
  scheme: bearer
  sources:
  - https://commodities.sh/docs/authentication
  type: http
slug: commodities-sh-authentication
source_filename: commodities-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commodities.sh/docs/authentication\ndocs: https://commodities.sh/docs/authentication\nnote: The OpenAPI (info.version 0.1.0) declares no securitySchemes; this profile is read from the docs authentication page.\nsummary:\n  types: [x402, http-bearer]\nschemes:\n- name: x402\n  type: x402\n  scheme: x402 (HTTP 402 Payment Required, USDC on Base)\n  description: \"Agents should use x402: probe a paid route, settle USDC on Base from the 402 challenge, retry with X-PAYMENT. No long-lived secret is required.\"\n  header: X-PAYMENT\n  network: eip155:8453\n  asset: USDC\n  sources: [https://commodities.sh/docs/authentication, https://commodities.sh/x402]\n- name: ProApiKey\n  type: http\n  scheme: bearer\n  description: \"Human operators buy Pro ($19/mo or $180/yr) at /get-started, receive a cs_live_… key once, and send Authorization: Bearer cs_live_… on paid routes. Each call debits credits (1 credit = $0.01 of list price).\
  \ Exhausted quota returns HTTP 402 QUOTA_EXCEEDED.\"\n  key_prefix: cs_live_\n  sources: [https://commodities.sh/docs/authentication]\n"
source_yaml_url: https://artifacts.apis.io/commodities-sh/authentication/commodities-sh-authentication.yml
summary_line: x402/http-bearer · 2 schemes
tags:
- Company
- Commodities
- Market Data
- Energy
- Agriculture
- Metals
- AI Agents
- MCP
- x402
- Government Data
---
