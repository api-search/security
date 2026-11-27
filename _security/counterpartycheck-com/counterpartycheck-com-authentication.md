---
anonymous_access: false
api_key_in: []
api_specs:
- filename: counterpartycheck-com-account-api-openapi.yml
  format: yaml
  label: Counterparty Check Account API
  slug: counterpartycheck-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-account-api-openapi.yml
- filename: counterpartycheck-com-check-api-openapi.yml
  format: yaml
  label: Counterparty Check Check API
  slug: counterpartycheck-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-check-api-openapi.yml
- filename: counterpartycheck-com-mcp-api-openapi.yml
  format: yaml
  label: Counterparty Check MCP API
  slug: counterpartycheck-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-mcp-api-openapi.yml
- filename: counterpartycheck-com-pricing-api-openapi.yml
  format: yaml
  label: Counterparty Check Pricing API
  slug: counterpartycheck-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-pricing-api-openapi.yml
- filename: counterpartycheck-com-receipts-api-openapi.yml
  format: yaml
  label: Counterparty Check Receipts API
  slug: counterpartycheck-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-receipts-api-openapi.yml
- filename: counterpartycheck-com-screen-api-openapi.yml
  format: yaml
  label: Counterparty Check Screen API
  slug: counterpartycheck-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/counterpartycheck-com/openapi/counterpartycheck-com-screen-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Counterparty Check Authentication
name_suffix: Authentication
oauth_flows: []
overview: Counterparty Check declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Counterparty Check
provider_slug: counterpartycheck-com
scheme_count: 3
schemes:
- description: Prepaid API key (cc_live_…), bought at /#pricing
  header: 'Authorization: Bearer cc_live_…'
  key_prefix: cc_live_
  name: apiKey
  obtain: Buy prepaid credit by card at https://counterpartycheck.com/#pricing; the key is issued immediately.
  scheme: bearer
  type: http
- description: No account. Call the endpoint without payment, get HTTP 402 with a PAYMENT-REQUIRED header, pay in USDC on Base (eip155:8453), retry with PAYMENT-SIGNATURE.
  documented_only: true
  name: x402
  type: payment
- description: 'Machine Payments Protocol: the same 402 carries a WWW-Authenticate: Payment challenge for USDC on Tempo.'
  documented_only: true
  name: mpp
  type: payment
slug: counterpartycheck-com-authentication
source_filename: counterpartycheck-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://counterpartycheck.com/docs\ndocs: https://counterpartycheck.com/docs\nspec: openapi/counterpartycheck-com-openapi.yml\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Prepaid API key (cc_live_…), bought at /#pricing\n  header: 'Authorization: Bearer cc_live_…'\n  key_prefix: cc_live_\n  obtain: Buy prepaid credit by card at https://counterpartycheck.com/#pricing; the key is issued immediately.\n- name: x402\n  type: payment\n  description: No account. Call the endpoint without payment, get HTTP 402 with a PAYMENT-REQUIRED header, pay in USDC on Base (eip155:8453), retry with PAYMENT-SIGNATURE.\n  documented_only: true\n- name: mpp\n  type: payment\n  description: 'Machine Payments Protocol: the same 402 carries a WWW-Authenticate: Payment challenge for USDC on Tempo.'\n  documented_only: true\nnotes:\n- The MCP server at https://counterpartycheck.com/mcp uses a prepaid API key; screen_sanctions\
  \ works without a key for 3 screens a day.\n- POST /v1/receipts/verify and GET /pricing are free and need no payment.\n"
source_yaml_url: https://artifacts.apis.io/counterpartycheck-com/authentication/counterpartycheck-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Payments
- Fraud Prevention
- Sanctions Screening
- Compliance
- AI Agents
- MCP
- x402
- Know Your Counterparty
---
