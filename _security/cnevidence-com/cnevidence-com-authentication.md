---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cnevidence-com-free-api-openapi.yml
  format: yaml
  label: CN Evidence Free API
  slug: cnevidence-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnevidence-com/openapi/cnevidence-com-free-api-openapi.yml
- filename: cnevidence-com-x402-api-openapi.yml
  format: yaml
  label: CN Evidence X402 API
  slug: cnevidence-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnevidence-com/openapi/cnevidence-com-x402-api-openapi.yml
auth_types:
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CN Evidence Authentication
name_suffix: Authentication
oauth_flows: []
overview: CN Evidence secures its APIs with x402-payment across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CN Evidence
provider_slug: cnevidence-com
scheme_count: 3
schemes:
- description: 'Paid /x402/* endpoints answer HTTP 402 Payment Required. The client signs an x402 v2 "exact" EVM payment in USDC on Base mainnet (eip155:8453) and resends the request. Docs: "Payment is x402 v2, exact, USDC on Base mainnet (eip155:8453), not Base Sepolia." and "当前没有预充值 API Key 方案" (there is currently no prepaid API-key option). Native MPP and the old the402 webhook are paused.'
  location: x402 v2 payment headers on the paid request
  name: x402-v2
  type: payment
- description: An optional secret the client generates itself (32 random bytes encoded as 64 lowercase hex). It is sent on the paid POST and later used in the body of POST /free/cn/payment/recover to fetch status or the report within 24 hours. This is a recovery credential, not an access key. The server stores only its hash.
  in: header
  name: X-CN-Recovery-Token
  type: apiKey
- description: The free catalog, product, preflight, compose, supplement and recovery endpoints take no API key.
  name: none
  type: none
slug: cnevidence-com-authentication
source_filename: cnevidence-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://yangchunhong3000.github.io/cn-evidence-public-docs/buyer-guide.html\ndocs: https://yangchunhong3000.github.io/cn-evidence-public-docs/buyer-guide.html\nsummary:\n  types:\n  - x402-payment\nnote: The OpenAPI (openapi/_original/cnevidence-com-openapi.json) declares no securitySchemes. Paid endpoints use HTTP x402 v2 payment rather than accounts or API keys. Free endpoints (/free/*) take no credentials.\nschemes:\n- name: x402-v2\n  type: payment\n  description: 'Paid /x402/* endpoints answer HTTP 402 Payment Required. The client signs an x402 v2 \"exact\" EVM payment in USDC on Base mainnet (eip155:8453) and resends the request. Docs: \"Payment is x402 v2, exact, USDC on Base mainnet (eip155:8453), not Base Sepolia.\" and \"当前没有预充值 API Key 方案\" (there is currently no prepaid API-key option). Native MPP and the old the402 webhook are paused.'\n  location: x402 v2 payment headers on the paid request\n- name: X-CN-Recovery-Token\n\
  \  type: apiKey\n  in: header\n  description: An optional secret the client generates itself (32 random bytes encoded as 64 lowercase hex). It is sent on the paid POST and later used in the body of POST /free/cn/payment/recover to fetch status or the report within 24 hours. This is a recovery credential, not an access key. The server stores only its hash.\n- name: none\n  type: none\n  description: The free catalog, product, preflight, compose, supplement and recovery endpoints take no API key.\n"
source_yaml_url: https://artifacts.apis.io/cnevidence-com/authentication/cnevidence-com-authentication.yml
summary_line: x402-payment · 3 schemes
tags:
- Company
- China
- Company Data
- Due Diligence
- Supplier Screening
- KYB
- x402
- Payments
- MCP
- Business Information
---
