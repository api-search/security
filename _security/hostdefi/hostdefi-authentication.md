---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hostdefi-token-risk-api-openapi.yml
  format: yaml
  label: HostDeFi Token Risk API
  slug: hostdefi-token-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-token-risk-api-openapi.yml
- filename: hostdefi-analyze-token-api-openapi.yml
  format: yaml
  label: HostDeFi Analyze Token API
  slug: hostdefi-analyze-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-analyze-token-api-openapi.yml
- filename: hostdefi-health-api-openapi.yml
  format: yaml
  label: HostDeFi Health API
  slug: hostdefi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-health-api-openapi.yml
- filename: hostdefi-keys-api-openapi.yml
  format: yaml
  label: HostDeFi Keys API
  slug: hostdefi-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-keys-api-openapi.yml
- filename: hostdefi-scan-api-openapi.yml
  format: yaml
  label: HostDeFi Scan API
  slug: hostdefi-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-scan-api-openapi.yml
- filename: hostdefi-usage-api-openapi.yml
  format: yaml
  label: HostDeFi Usage API
  slug: hostdefi-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-usage-api-openapi.yml
- filename: hostdefi-x402-machine-payable-api-openapi.yml
  format: yaml
  label: HostDeFi x402 (machine-payable) API
  slug: hostdefi-x402-machine-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-x402-machine-payable-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hostdefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: HostDeFi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HostDeFi
provider_slug: hostdefi
scheme_count: 1
schemes:
- description: API key from POST /v1/keys (vx_ + 32 hex chars). Omit it to use the keyless free tier (100 calls/day per IP).
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/hostdefi-analyze-token-api-openapi.yml
  - openapi/hostdefi-health-api-openapi.yml
  - openapi/hostdefi-keys-api-openapi.yml
  - openapi/hostdefi-scan-api-openapi.yml
  - openapi/hostdefi-token-risk-api-openapi.yml
  - openapi/hostdefi-usage-api-openapi.yml
  - openapi/hostdefi-x402-machine-payable-api-openapi.yml
  type: apiKey
slug: hostdefi-authentication
source_filename: hostdefi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/hostdefi-analyze-token-api-openapi.yml, openapi/hostdefi-health-api-openapi.yml,\n  openapi/hostdefi-keys-api-openapi.yml, openapi/hostdefi-scan-api-openapi.yml, openapi/hostdefi-token-risk-api-openapi.yml,\n  openapi/hostdefi-usage-api-openapi.yml, openapi/hostdefi-x402-machine-payable-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from POST /v1/keys (vx_ + 32 hex chars). Omit it to use the keyless free\n    tier (100 calls/day per IP).\n  sources:\n  - openapi/hostdefi-analyze-token-api-openapi.yml\n  - openapi/hostdefi-health-api-openapi.yml\n  - openapi/hostdefi-keys-api-openapi.yml\n  - openapi/hostdefi-scan-api-openapi.yml\n  - openapi/hostdefi-token-risk-api-openapi.yml\n  - openapi/hostdefi-usage-api-openapi.yml\n  - openapi/hostdefi-x402-machine-payable-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/authentication/hostdefi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Solana
- Token Risk
- DeFi
- rug pull
- x402
---
