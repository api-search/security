---
anonymous_access: true
api_key_in: []
api_specs:
- filename: clinkforge-com-openapi-generated.yml
  format: yaml
  label: Clink Forge API
  slug: clinkforge-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clinkforge-com/openapi/_ae-authored/clinkforge-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clink Forge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clink Forge declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Clink Forge
provider_slug: clinkforge-com
scheme_count: 3
schemes:
- description: 'An unpaid GET /v1/p/<slug> returns 402 Payment Required with the terms "in both protocol generations: the x402 v1 JSON body and the canonical v2 PAYMENT-REQUIRED header". The client signs an EIP-3009 transferWithAuthorization for USDC on Base and retries with X-PAYMENT: <signed>. The 200 response carries the settlement in X-PAYMENT-RESPONSE.'
  header: X-PAYMENT
  in: header
  name: x402-payment
  type: x402
  x-kind: x402-payment
- description: 'Over MCP (https://api.clinkforge.com/mcp), a paid tool returns isError: true with an x402 PaymentRequired object. The client retries with the payment in _meta["x402/payment"], and the settlement comes back in _meta["x402/payment-response"]. initialize, tools/list, ping and search_catalog never require payment.'
  name: x402-mcp
  type: x402-mcp-transport
- description: Verification (POST /v1/verify/attestation, GET /v1/meta/keys) and the discovery surfaces are free and need no account.
  name: none
  type: none
slug: clinkforge-com-authentication
source_filename: clinkforge-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clinkforge.com/docs/\ndocs: https://clinkforge.com/docs/\nsummary: 'There are no credentials: \"no account, no API key, no subscription\". Access is paid per request through the x402 HTTP payment protocol. The client sends the signed payment in a request header (HTTP) or in _meta (MCP).'\nschemes:\n- name: x402-payment\n  type: x402\n  in: header\n  header: X-PAYMENT\n  x-kind: x402-payment\n  description: 'An unpaid GET /v1/p/<slug> returns 402 Payment Required with the terms \"in both protocol generations: the x402 v1 JSON body and the canonical v2 PAYMENT-REQUIRED header\". The client signs an EIP-3009 transferWithAuthorization for USDC on Base and retries with X-PAYMENT: <signed>. The 200 response carries the settlement in X-PAYMENT-RESPONSE.'\n- name: x402-mcp\n  type: x402-mcp-transport\n  description: 'Over MCP (https://api.clinkforge.com/mcp), a paid tool returns isError: true with an x402 PaymentRequired object.\
  \ The client retries with the payment in _meta[\"x402/payment\"], and the settlement comes back in _meta[\"x402/payment-response\"]. initialize, tools/list, ping and search_catalog never require payment.'\n- name: none\n  type: none\n  description: Verification (POST /v1/verify/attestation, GET /v1/meta/keys) and the discovery surfaces are free and need no account.\n"
source_yaml_url: https://artifacts.apis.io/clinkforge-com/authentication/clinkforge-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Government Data
- Open Data
- x402
- Payments
- MCP
- AI Agents
- Data Provenance
- Cryptocurrency
---
