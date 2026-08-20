---
api_key_in: []
api_specs:
- filename: waodao-artchain-api-openapi.yml
  format: yaml
  label: WAODAO Art Chain API
  slug: waodao-artchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-artchain-api-openapi.yml
- filename: waodao-liquidity-pools-api-openapi.yml
  format: yaml
  label: WAODAO Liquidity Pools API
  slug: waodao-liquidity-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-liquidity-pools-api-openapi.yml
- filename: waodao-schema-api-openapi.yml
  format: yaml
  label: WAODAO Schema API
  slug: waodao-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-schema-api-openapi.yml
- filename: waodao-token-metadata-api-openapi.yml
  format: yaml
  label: WAODAO Token Metadata API
  slug: waodao-token-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-token-metadata-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Waodao Authentication
name_suffix: Authentication
oauth_flows: []
overview: WAODAO secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WAODAO
provider_slug: waodao
scheme_count: 0
schemes: []
slug: waodao-authentication
source_filename: waodao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://waodao.ai/ai-agents#api-access\ndocs: https://waodao.ai/ai-agents\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public: true\nschemes: []\nposture:\n  authentication_required: false\n  statement: >-\n    \"The API is public and free to read: no account, API key, payment, or authentication is\n    required. CORS is enabled.\" — WAODAO AI agent documentation (api-access section) and\n    llms.txt Access Notes.\n  cors:\n    enabled: true\n    header: 'Access-Control-Allow-Origin: *'\n    observed: true\n  spec_evidence: >-\n    openapi/waodao-agent-api-openapi.json declares an empty root `security: []` and an empty\n    `components.securitySchemes`, which matches the documented no-auth posture rather than\n    indicating an undocumented scheme.\n  scopes: none\n  note: >-\n    All five operations are read-only GETs over public NFT/ArtChain metadata and public on-chain\n    pool registry data, so\
  \ there is no OAuth scope surface. scopes/ is intentionally absent.\ncontact: info@waodao.ai\ncross_links:\n  conventions: conventions/waodao-conventions.yml\n  conformance: conformance/waodao-conformance.yml\n  openapi: openapi/waodao-agent-api-openapi.json\nx-evidence:\n  - {url: 'https://waodao.ai/ai-agents', http_status: 200}\n  - {url: 'https://waodao.ai/llms.txt', http_status: 200}\n  - {url: 'https://waodao.ai/api/v1/waodao/index', http_status: 200, note: 'returned 200 with no credentials; access-control-allow-origin: *'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/authentication/waodao-authentication.yml
summary_line: none · 0 schemes
tags:
- AI Agents
- ArtChain
- Human and AI
- NFT Metadata
- On-chain Culture
- Liquidity Pools
- Web3
- OpenAPI
- Ethereum
- Solana
- agent-native
- Digital Art
---
