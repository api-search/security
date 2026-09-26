---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kronos-seshat-agent-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent API
  slug: kronos-seshat-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-api-openapi.yml
- filename: kronos-seshat-agent-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent Intelligence API
  slug: kronos-seshat-agent-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-intelligence-api-openapi.yml
- filename: kronos-seshat-analysis-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Analysis API
  slug: kronos-seshat-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-analysis-api-openapi.yml
- filename: kronos-seshat-discovery-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Discovery API
  slug: kronos-seshat-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-discovery-api-openapi.yml
- filename: kronos-seshat-experimental-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Experimental API
  slug: kronos-seshat-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-experimental-api-openapi.yml
- filename: kronos-seshat-forecast-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Forecast API
  slug: kronos-seshat-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-forecast-api-openapi.yml
- filename: kronos-seshat-market-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Market Intelligence API
  slug: kronos-seshat-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-market-intelligence-api-openapi.yml
- filename: kronos-seshat-semantic-similarity-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Semantic Similarity API
  slug: kronos-seshat-semantic-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-semantic-similarity-api-openapi.yml
- filename: kronos-seshat-signal-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Signal API
  slug: kronos-seshat-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-signal-api-openapi.yml
- filename: kronos-seshat-verification-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Verification API
  slug: kronos-seshat-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-verification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kronos Seshat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kronos Quant Signal API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kronos Quant Signal API
provider_slug: kronos-seshat
scheme_count: 1
schemes:
- description: x402 v2 payment payload. Required for paid endpoints when the service manifest at /.well-known/x402 has enforcement=active_mainnet. Send the signed payment in this header (or the legacy X-PAYMENT header) to satisfy the 402 challenge.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/kronos-seshat-openapi.json
  type: apiKey
slug: kronos-seshat-authentication
source_filename: kronos-seshat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/kronos-seshat-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 payment payload. Required for paid endpoints when the service manifest\n    at /.well-known/x402 has enforcement=active_mainnet. Send the signed payment in this header\n    (or the legacy X-PAYMENT header) to satisfy the 402 challenge.\n  sources:\n  - openapi/kronos-seshat-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/authentication/kronos-seshat-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crypto
- Financial Forecast
- API
- Market Data
- Auditing
- Micropayments
---
