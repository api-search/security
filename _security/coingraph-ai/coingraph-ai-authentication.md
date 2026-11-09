---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coingraph-ai-agents-api-openapi.yml
  format: yaml
  label: CoinGraph Agents API
  slug: coingraph-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-agents-api-openapi.yml
- filename: coingraph-ai-decide-api-openapi.yml
  format: yaml
  label: CoinGraph Decide API
  slug: coingraph-ai-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-decide-api-openapi.yml
- filename: coingraph-ai-discover-api-openapi.yml
  format: yaml
  label: CoinGraph Discover API
  slug: coingraph-ai-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-discover-api-openapi.yml
- filename: coingraph-ai-trust-api-openapi.yml
  format: yaml
  label: CoinGraph Trust API
  slug: coingraph-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-trust-api-openapi.yml
- filename: coingraph-ai-understand-api-openapi.yml
  format: yaml
  label: CoinGraph Understand API
  slug: coingraph-ai-understand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-understand-api-openapi.yml
- filename: coingraph-ai-watch-api-openapi.yml
  format: yaml
  label: CoinGraph Watch API
  slug: coingraph-ai-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-watch-api-openapi.yml
auth_types: []
description: Authentication schemes for CoinGraph API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Coingraph Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinGraph declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CoinGraph
provider_slug: coingraph-ai
scheme_count: 3
schemes:
- evidence: Auth None
  name: None
  type: other
- evidence: 'with a key, send Authorization: Bearer cg_live_…'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Auth Key or x402 after 25 a day
  name: Key or x402
  type: other
slug: coingraph-ai-authentication
source_filename: coingraph-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://coingraph.ai/docs/api/tokens
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://coingraph.ai/docs/api/tokens\nsources:\n- https://coingraph.ai/docs/api/tokens\n- https://coingraph.ai/docs/api/state\n- https://coingraph.ai/docs/api/history\n- https://coingraph.ai/docs/api/evaluate\ndescription: Authentication schemes for CoinGraph API\nschemes:\n- type: other\n  name: None\n  evidence: Auth None\n- type: http-bearer\n  name: Bearer token\n  evidence: 'with a key, send Authorization: Bearer cg_live_…'\n  location: header\n  header: Authorization\n- type: other\n  name: Key or x402\n  evidence: Auth Key or x402 after 25 a day\ndocs: https://coingraph.ai/docs/api/tokens\n"
source_yaml_url: https://artifacts.apis.io/coingraph-ai/authentication/coingraph-ai-authentication.yml
summary_line: 3 schemes
tags:
- Crypto Data
- AI Agents
- trading agents
- Wallets
- On-Chain Data
- Market Data
---
