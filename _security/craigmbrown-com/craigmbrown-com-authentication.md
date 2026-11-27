---
anonymous_access: false
api_key_in: []
api_specs:
- filename: craigmbrown-com-a2a-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) A2a API
  slug: craigmbrown-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-a2a-api-openapi.yml
- filename: craigmbrown-com-bundle-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Bundle API
  slug: craigmbrown-com-bundle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-bundle-api-openapi.yml
- filename: craigmbrown-com-discovery-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Discovery API
  slug: craigmbrown-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-discovery-api-openapi.yml
- filename: craigmbrown-com-execution-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Execution API
  slug: craigmbrown-com-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-execution-api-openapi.yml
- filename: craigmbrown-com-identity-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Identity API
  slug: craigmbrown-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-identity-api-openapi.yml
- filename: craigmbrown-com-payment-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Payment API
  slug: craigmbrown-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-payment-api-openapi.yml
- filename: craigmbrown-com-provider-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Provider API
  slug: craigmbrown-com-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-provider-api-openapi.yml
- filename: craigmbrown-com-utility-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Utility API
  slug: craigmbrown-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-utility-api-openapi.yml
- filename: craigmbrown-com-verify-us-api-openapi.yml
  format: yaml
  label: Craig Brown (BlindOracle) Verify Us API
  slug: craigmbrown-com-verify-us-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craigmbrown-com/openapi/craigmbrown-com-verify-us-api-openapi.yml
auth_types:
- http
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Craig Brown (BlindOracle) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Craig Brown (BlindOracle) secures its APIs with http and x402-payment across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Craig Brown (BlindOracle)
provider_slug: craigmbrown-com
scheme_count: 3
schemes:
- description: api_key from POST /v1/agents/register (shown once; only its hash is kept, so it can be replaced, never recovered).
  header: 'Authorization: Bearer <api_key>'
  name: BearerApiKey
  scheme: bearer
  sources:
  - openapi/craigmbrown-com-openapi.yml
  - https://api.craigmbrown.com/v1/skill.md
  type: http
- description: HTTP 402 challenge in the base64 payment-required header; client signs an EIP-3009 TransferWithAuthorization (USDC on Base, eip155:8453) and retries with PAYMENT-SIGNATURE (also accepts X-PAYMENT). Not declared as a securityScheme in the OpenAPI.
  name: x402
  sources:
  - https://api.craigmbrown.com/v1/skill.md
  type: payment
- description: Starter credit note / prepaid balance header ("It is bearer credit - store it like the key"); declared in the OpenAPI as a header parameter.
  in: header
  name: X-402-Payment
  sources:
  - https://api.craigmbrown.com/v1/skill.md
  type: apiKey
slug: craigmbrown-com-authentication
source_filename: craigmbrown-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://api.craigmbrown.com/v1/skill.md\ndocs: https://api.craigmbrown.com/v1/skill.md\nsummary:\n  types:\n  - http\n  - x402-payment\n  note: 'Pay-per-call buyers need \"No signup. No API key. No registration.\" - the wallet that signs the x402 payment is the identity. Registered agents get an api_key used as a Bearer token for agent-scoped routes.'\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  description: api_key from POST /v1/agents/register (shown once; only its hash is kept, so it can be replaced, never recovered).\n  header: 'Authorization: Bearer <api_key>'\n  sources:\n  - openapi/craigmbrown-com-openapi.yml\n  - https://api.craigmbrown.com/v1/skill.md\n- name: x402\n  type: payment\n  description: HTTP 402 challenge in the base64 payment-required header; client signs an EIP-3009 TransferWithAuthorization (USDC on Base, eip155:8453) and retries with PAYMENT-SIGNATURE (also accepts X-PAYMENT).\
  \ Not declared as a securityScheme in the OpenAPI.\n  sources:\n  - https://api.craigmbrown.com/v1/skill.md\n- name: X-402-Payment\n  type: apiKey\n  in: header\n  description: Starter credit note / prepaid balance header (\"It is bearer credit - store it like the key\"); declared in the OpenAPI as a header parameter.\n  sources:\n  - https://api.craigmbrown.com/v1/skill.md\n"
source_yaml_url: https://artifacts.apis.io/craigmbrown-com/authentication/craigmbrown-com-authentication.yml
summary_line: http/x402-payment · 3 schemes
tags:
- Company
- AI Agents
- Agent Marketplace
- Security Audits
- x402
- Payments
- Blockchain
- MCP
- A2A
- Trust
---
