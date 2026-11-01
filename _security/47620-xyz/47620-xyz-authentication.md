---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 47620-xyz-agent-api-openapi.yml
  format: yaml
  label: 47620-xyz Agent API
  slug: 47620-xyz-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-agent-api-openapi.yml
- filename: 47620-xyz-agent-commerce-api-openapi.yml
  format: yaml
  label: 47620-xyz Agent Commerce API
  slug: 47620-xyz-agent-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-agent-commerce-api-openapi.yml
- filename: 47620-xyz-base-api-openapi.yml
  format: yaml
  label: 47620-xyz Base API
  slug: 47620-xyz-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-base-api-openapi.yml
- filename: 47620-xyz-blockchain-data-api-openapi.yml
  format: yaml
  label: 47620-xyz Blockchain Data API
  slug: 47620-xyz-blockchain-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-blockchain-data-api-openapi.yml
- filename: 47620-xyz-catalog-api-openapi.yml
  format: yaml
  label: 47620-xyz Catalog API
  slug: 47620-xyz-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-catalog-api-openapi.yml
- filename: 47620-xyz-crypto-api-openapi.yml
  format: yaml
  label: 47620-xyz Crypto API
  slug: 47620-xyz-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-crypto-api-openapi.yml
- filename: 47620-xyz-data-api-openapi.yml
  format: yaml
  label: 47620-xyz Data API
  slug: 47620-xyz-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-data-api-openapi.yml
- filename: 47620-xyz-discovery-api-openapi.yml
  format: yaml
  label: 47620-xyz Discovery API
  slug: 47620-xyz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-discovery-api-openapi.yml
- filename: 47620-xyz-mcp-api-openapi.yml
  format: yaml
  label: 47620-xyz MCP API
  slug: 47620-xyz-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-mcp-api-openapi.yml
- filename: 47620-xyz-nano-api-openapi.yml
  format: yaml
  label: 47620-xyz Nano API
  slug: 47620-xyz-nano-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-nano-api-openapi.yml
- filename: 47620-xyz-polygon-api-openapi.yml
  format: yaml
  label: 47620-xyz Polygon API
  slug: 47620-xyz-polygon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-polygon-api-openapi.yml
- filename: 47620-xyz-security-api-openapi.yml
  format: yaml
  label: 47620-xyz Security API
  slug: 47620-xyz-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-security-api-openapi.yml
- filename: 47620-xyz-trust-api-openapi.yml
  format: yaml
  label: 47620-xyz Trust API
  slug: 47620-xyz-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-trust-api-openapi.yml
- filename: 47620-xyz-underwriting-api-openapi.yml
  format: yaml
  label: 47620-xyz Underwriting API
  slug: 47620-xyz-underwriting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-underwriting-api-openapi.yml
- filename: 47620-xyz-utilities-api-openapi.yml
  format: yaml
  label: 47620-xyz Utilities API
  slug: 47620-xyz-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-utilities-api-openapi.yml
- filename: 47620-xyz-x402-api-openapi.yml
  format: yaml
  label: 47620-xyz X402 API
  slug: 47620-xyz-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/47620-xyz/openapi/47620-xyz-x402-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 47620 Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: 47620-xyz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 47620-xyz
provider_slug: 47620-xyz
scheme_count: 1
schemes:
- description: Sign-In with X wallet proof (used by registries; not required to buy).
  in: header
  name: siwx
  parameter: X-SIWX
  sources:
  - openapi/47620-xyz-openapi.yml
  - openapi/openapi.json
  type: apiKey
slug: 47620-xyz-authentication
source_filename: 47620-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/47620-xyz-openapi.yml, openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: X-SIWX\n  description: Sign-In with X wallet proof (used by registries; not required to buy).\n  sources:\n  - openapi/47620-xyz-openapi.yml\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/47620-xyz/authentication/47620-xyz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FinTech
- Payments
- Blockchain
- Solana
- API
---
