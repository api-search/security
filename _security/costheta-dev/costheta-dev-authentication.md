---
anonymous_access: true
api_key_in: []
api_specs:
- filename: costheta-dev-dada-api-openapi.yml
  format: yaml
  label: costheta Dada API
  slug: costheta-dev-dada-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-dada-api-openapi.yml
- filename: costheta-dev-fastapi-api-openapi.yml
  format: yaml
  label: costheta Fast API
  slug: costheta-dev-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-fastapi-api-openapi.yml
- filename: costheta-dev-federation-api-openapi.yml
  format: yaml
  label: costheta Federation API
  slug: costheta-dev-federation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-federation-api-openapi.yml
- filename: costheta-dev-keys-api-openapi.yml
  format: yaml
  label: costheta Keys API
  slug: costheta-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-keys-api-openapi.yml
- filename: costheta-dev-llms-txt-api-openapi.yml
  format: yaml
  label: costheta Llms.txt API
  slug: costheta-dev-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-llms-txt-api-openapi.yml
- filename: costheta-dev-mcp-api-openapi.yml
  format: yaml
  label: costheta MCP API
  slug: costheta-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-mcp-api-openapi.yml
- filename: costheta-dev-muon-api-openapi.yml
  format: yaml
  label: costheta Muon API
  slug: costheta-dev-muon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-muon-api-openapi.yml
- filename: costheta-dev-pulse-api-openapi.yml
  format: yaml
  label: costheta Pulse API
  slug: costheta-dev-pulse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-pulse-api-openapi.yml
- filename: costheta-dev-state-api-openapi.yml
  format: yaml
  label: costheta State API
  slug: costheta-dev-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-state-api-openapi.yml
- filename: costheta-dev-stream-api-openapi.yml
  format: yaml
  label: costheta Stream API
  slug: costheta-dev-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-stream-api-openapi.yml
- filename: costheta-dev-support-js-api-openapi.yml
  format: yaml
  label: costheta Support.js API
  slug: costheta-dev-support-js-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-support-js-api-openapi.yml
- filename: costheta-dev-v-api-openapi.yml
  format: yaml
  label: costheta V API
  slug: costheta-dev-v-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-v-api-openapi.yml
- filename: costheta-dev-why-api-openapi.yml
  format: yaml
  label: costheta Why API
  slug: costheta-dev-why-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costheta-dev/openapi/costheta-dev-why-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: costheta Authentication
name_suffix: Authentication
oauth_flows: []
overview: costheta declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: costheta
provider_slug: costheta-dev
scheme_count: 2
schemes:
- applies_to: public endpoints (GET /pulse/latest, /stream, /keys, /v/{muon_id}, /state) and the free costheta_random MCP tool
  evidence: 'costheta_random: free public beacon derived from the latest signed detector pulse.'
  name: none
  type: none
- description: Per-call payment settled in USDC via x402 on Base mainnet, used instead of credentials for costheta_decide and costheta_witness.
  evidence: 'Paid tools: $0.02 per call, settled in USDC via x402.'
  name: x402
  type: payment
slug: costheta-dev-authentication
source_filename: costheta-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://costheta.dev/llms.txt\ndocs: https://costheta.dev/llms.txt\nsummary: No accounts or API keys. Free endpoints (beacon, stream, keys, certificate verification) are open; paid MCP tools are paid per call via the x402 HTTP 402 payment protocol in USDC on Base mainnet. The OpenAPI document declares no securitySchemes.\nschemes:\n- name: none\n  type: none\n  applies_to: public endpoints (GET /pulse/latest, /stream, /keys, /v/{muon_id}, /state) and the free costheta_random MCP tool\n  evidence: 'costheta_random: free public beacon derived from the latest signed detector pulse.'\n- name: x402\n  type: payment\n  description: Per-call payment settled in USDC via x402 on Base mainnet, used instead of credentials for costheta_decide and costheta_witness.\n  evidence: 'Paid tools: $0.02 per call, settled in USDC via x402.'\n"
source_yaml_url: https://artifacts.apis.io/costheta-dev/authentication/costheta-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Randomness
- Verifiable Randomness
- Cryptography
- Post-Quantum Cryptography
- AI Agents
- MCP
- x402
---
