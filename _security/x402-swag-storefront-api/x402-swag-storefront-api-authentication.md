---
anonymous_access: false
api_key_in: []
api_specs:
- filename: x402-swag-storefront-api-openapi.json
  format: json
  label: x402 Swag storefront API
  slug: x402-swag-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x402-swag-storefront-api/refs/heads/main/openapi/x402-swag-storefront-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: X402 Swag Storefront Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: x402 Swag storefront API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: x402 Swag storefront API
provider_slug: x402-swag-storefront-api
scheme_count: 0
schemes: []
slug: x402-swag-storefront-api-authentication
source_filename: x402-swag-storefront-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi (no securitySchemes) + /.well-known/agent-card.json + /.well-known/x402.json\nschemes: []\nmodel: none / payment-gated\nnote: 'OpenAPI declares no securitySchemes; no API keys or accounts. Browsing (products, collections,\n  cart, checkout rates) is free and unauthenticated. Paid routes are gated by x402: server answers HTTP\n  402 with payment terms (USDC on Base, eip155:8453) and the caller pays and retries with a payment/signature\n  header. This is payment gating, not authentication.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-swag-storefront-api/refs/heads/main/authentication/x402-swag-storefront-api-authentication.yml
summary_line: 0 schemes
tags:
- e-commerce
- retail
- merchandise
- agentic commerce
- x402
- crypto payments
- stablecoin
- USDC
- Base
- onchain
- machine-payable API
- print-on-demand
---
