---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kairossignal-com-brief-api-openapi.yml
  format: yaml
  label: kairossignal-com Brief API
  slug: kairossignal-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-brief-api-openapi.yml
- filename: kairossignal-com-credits-api-openapi.yml
  format: yaml
  label: kairossignal-com Credits API
  slug: kairossignal-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-credits-api-openapi.yml
- filename: kairossignal-com-export-api-openapi.yml
  format: yaml
  label: kairossignal-com Export API
  slug: kairossignal-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-export-api-openapi.yml
- filename: kairossignal-com-market-api-openapi.yml
  format: yaml
  label: kairossignal-com Market API
  slug: kairossignal-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-market-api-openapi.yml
- filename: kairossignal-com-mcp-api-openapi.yml
  format: yaml
  label: kairossignal-com MCP API
  slug: kairossignal-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-mcp-api-openapi.yml
- filename: kairossignal-com-network-api-openapi.yml
  format: yaml
  label: kairossignal-com Network API
  slug: kairossignal-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-network-api-openapi.yml
- filename: kairossignal-com-networks-api-openapi.yml
  format: yaml
  label: kairossignal-com Networks API
  slug: kairossignal-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-networks-api-openapi.yml
- filename: kairossignal-com-provenance-api-openapi.yml
  format: yaml
  label: kairossignal-com Provenance API
  slug: kairossignal-com-provenance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-provenance-api-openapi.yml
- filename: kairossignal-com-revenue-api-openapi.yml
  format: yaml
  label: kairossignal-com Revenue API
  slug: kairossignal-com-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-revenue-api-openapi.yml
- filename: kairossignal-com-supply-api-openapi.yml
  format: yaml
  label: kairossignal-com Supply API
  slug: kairossignal-com-supply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-supply-api-openapi.yml
- filename: kairossignal-com-try-api-openapi.yml
  format: yaml
  label: kairossignal-com Try API
  slug: kairossignal-com-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-try-api-openapi.yml
- filename: kairossignal-com-x402-api-openapi.yml
  format: yaml
  label: kairossignal-com X402 API
  slug: kairossignal-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-x402-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kairossignal Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: kairossignal-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kairossignal-com
provider_slug: kairossignal-com
scheme_count: 2
schemes:
- description: API key passed in X-API-Key header.
  in: header
  name: X-API-Key
  notes: Keys issued via POST /v1/credits/register or Stripe checkout. No OAuth.
  type: apiKey
- description: Ed25519 signed responses via X-Kairos-Signature, X-Kairos-Timestamp, X-Kairos-Signing-Key headers.
  name: Response Receipts
  type: custom
slug: kairossignal-com-authentication
source_filename: kairossignal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://kairossignal.com/docs/customer.html#auth\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key passed in X-API-Key header.\n    notes: Keys issued via POST /v1/credits/register or Stripe checkout. No OAuth.\n  - type: custom\n    name: Response Receipts\n    description: Ed25519 signed responses via X-Kairos-Signature, X-Kairos-Timestamp, X-Kairos-Signing-Key headers.\n"
source_yaml_url: https://artifacts.apis.io/kairossignal-com/authentication/kairossignal-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DePIN
- DataAPI
- Crypto
- Telemetry
- Analytics
---
