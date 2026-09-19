---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arakel-certificate-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Certificate API
  slug: arakel-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-certificate-api-openapi.yml
- filename: arakel-coverage-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Coverage API
  slug: arakel-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-coverage-api-openapi.yml
- filename: arakel-coverage-status-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Coverage Status API
  slug: arakel-coverage-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-coverage-status-api-openapi.yml
- filename: arakel-crypto-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Crypto API
  slug: arakel-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-crypto-api-openapi.yml
- filename: arakel-evidence-bundle-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Evidence Bundle API
  slug: arakel-evidence-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-evidence-bundle-api-openapi.yml
- filename: arakel-government-data-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Government Data API
  slug: arakel-government-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-government-data-api-openapi.yml
- filename: arakel-health-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Health API
  slug: arakel-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-health-api-openapi.yml
- filename: arakel-machine-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Machine API
  slug: arakel-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-machine-api-openapi.yml
- filename: arakel-quote-api-openapi.yml
  format: yaml
  label: ARAKEL Machine Evidence Network Quote API
  slug: arakel-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/openapi/arakel-quote-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arakel Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARAKEL Machine Evidence Network declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ARAKEL Machine Evidence Network
provider_slug: arakel
scheme_count: 1
schemes:
- asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
  asset_name: USD Coin (USDC)
  evidence:
    amount_atomic: '5000'
    amount_usd: 0.005
    http_status: 402
    url: https://proof.arakelproof.space/v1/ofac-sanctions-screening?q=OpenAI
  max_timeout_seconds: 300
  network: eip155:8453
  network_name: Base
  pay_to: '0x3a2F36D61c9BB3b3ee72426e2B6b58d774605B5e'
  scheme: exact
  spec_version: 2
  transport: HTTP 402 + payment-required header (base64url JSON) and payment-required response body
  type: x402
slug: arakel-authentication
source_filename: arakel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://proof.arakelproof.space/openapi.json (no securitySchemes),\n  https://proof.arakelproof.space/.well-known/x402,\n  live HTTP 402 challenge on GET /v1/ofac-sanctions-screening,\n  https://proof.arakelproof.space/skill.md, /terms\nname: ARAKEL Machine Evidence Network\nmodel: payment-gated (x402)\napi_keys: false\noauth2: false\nnote: >-\n  There are no API keys, OAuth, or securitySchemes. Authentication is identity-free\n  and payment-based: free preflight/quote routes are open, and paid product routes\n  answer HTTP 402 with an x402 v2 payment challenge that the caller settles with a\n  signed on-chain USDC transfer. Possession of a funded, x402-capable wallet is the\n  only credential.\nschemes:\n  - type: x402\n    spec_version: 2\n    transport: HTTP 402 + payment-required header (base64url JSON) and payment-required response body\n    network: eip155:8453\n    network_name: Base\n    asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n\
  \    asset_name: USD Coin (USDC)\n    scheme: exact\n    pay_to: '0x3a2F36D61c9BB3b3ee72426e2B6b58d774605B5e'\n    max_timeout_seconds: 300\n    evidence:\n      url: https://proof.arakelproof.space/v1/ofac-sanctions-screening?q=OpenAI\n      http_status: 402\n      amount_atomic: '5000'\n      amount_usd: 0.005\nfree_routes:\n  - /health\n  - /v1/coverage\n  - /v1/coverage-status\n  - /v1/quote\n  - /v1/machine/catalog\n  - /v1/machine/sources\n  - /v1/machine/sales-telemetry\n  - /v1/machine/quote\n  - /v1/machine/lookup-quote\n  - /v1/machine/counterparty-quote\n  - /v1/machine/counterparty-check-quote\n  - /v1/machine/batch-quote\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arakel/refs/heads/main/authentication/arakel-authentication.yml
summary_line: 1 scheme
tags:
- machine-evidence
- Compliance
- Sanctions Screening
- OFAC
- Regulatory Monitoring
- Government Data
- FDA-recalls
- Federal Spending
- Federal Register
- counterparty-due-diligence
- agent-native
- x402
- pay-per-call
- MCP
- A2A
---
