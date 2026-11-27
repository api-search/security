---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getchord-xyz-account-and-health-api-openapi.yml
  format: yaml
  label: Chord Account and health API
  slug: getchord-xyz-account-and-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-account-and-health-api-openapi.yml
- filename: getchord-xyz-agents-and-status-api-openapi.yml
  format: yaml
  label: Chord Agents and status API
  slug: getchord-xyz-agents-and-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-agents-and-status-api-openapi.yml
- filename: getchord-xyz-arc-data-api-openapi.yml
  format: yaml
  label: Chord Arc data API
  slug: getchord-xyz-arc-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-arc-data-api-openapi.yml
- filename: getchord-xyz-ask-agent-api-openapi.yml
  format: yaml
  label: Chord Ask agent API
  slug: getchord-xyz-ask-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-ask-agent-api-openapi.yml
- filename: getchord-xyz-avalanche-base-bnb-chain-api-openapi.yml
  format: yaml
  label: Chord Avalanche, Base, BNB Chain API
  slug: getchord-xyz-avalanche-base-bnb-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-avalanche-base-bnb-chain-api-openapi.yml
- filename: getchord-xyz-backtests-api-openapi.yml
  format: yaml
  label: Chord Backtests API
  slug: getchord-xyz-backtests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-backtests-api-openapi.yml
- filename: getchord-xyz-bridge-api-openapi.yml
  format: yaml
  label: Chord Bridge API
  slug: getchord-xyz-bridge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-bridge-api-openapi.yml
- filename: getchord-xyz-liquidity-api-openapi.yml
  format: yaml
  label: Chord Liquidity API
  slug: getchord-xyz-liquidity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-liquidity-api-openapi.yml
- filename: getchord-xyz-meta-aggregator-api-openapi.yml
  format: yaml
  label: Chord Meta aggregator API
  slug: getchord-xyz-meta-aggregator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-meta-aggregator-api-openapi.yml
- filename: getchord-xyz-points-api-openapi.yml
  format: yaml
  label: Chord Points API
  slug: getchord-xyz-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-points-api-openapi.yml
- filename: getchord-xyz-portfolio-api-openapi.yml
  format: yaml
  label: Chord Portfolio API
  slug: getchord-xyz-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-portfolio-api-openapi.yml
- filename: getchord-xyz-quote-and-swap-api-openapi.yml
  format: yaml
  label: Chord Quote and swap API
  slug: getchord-xyz-quote-and-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-quote-and-swap-api-openapi.yml
- filename: getchord-xyz-robinhood-chain-data-api-openapi.yml
  format: yaml
  label: Chord Robinhood Chain data API
  slug: getchord-xyz-robinhood-chain-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-robinhood-chain-data-api-openapi.yml
- filename: getchord-xyz-solana-data-api-openapi.yml
  format: yaml
  label: Chord Solana data API
  slug: getchord-xyz-solana-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-solana-data-api-openapi.yml
- filename: getchord-xyz-solana-swaps-api-openapi.yml
  format: yaml
  label: Chord Solana swaps API
  slug: getchord-xyz-solana-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-solana-swaps-api-openapi.yml
- filename: getchord-xyz-streaming-api-openapi.yml
  format: yaml
  label: Chord Streaming API
  slug: getchord-xyz-streaming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-streaming-api-openapi.yml
- filename: getchord-xyz-token-safety-api-openapi.yml
  format: yaml
  label: Chord Token safety API
  slug: getchord-xyz-token-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-token-safety-api-openapi.yml
- filename: getchord-xyz-tokens-and-charts-api-openapi.yml
  format: yaml
  label: Chord Tokens and charts API
  slug: getchord-xyz-tokens-and-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-tokens-and-charts-api-openapi.yml
- filename: getchord-xyz-top-wallets-api-openapi.yml
  format: yaml
  label: Chord Top wallets API
  slug: getchord-xyz-top-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getchord-xyz/openapi/getchord-xyz-top-wallets-api-openapi.yml
auth_types: []
description: Chord uses an API key sent in the X-API-Key request header. A Google‑session bearer token can also be used for the Ask agent API, but the documented primary authentication is the API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chord Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chord declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chord
provider_slug: getchord-xyz
scheme_count: 1
schemes:
- evidence: POST /v1/ask — the Ask agent API (a Google session bearer also works; that is what the browser uses).
  header: Authorization
  how_to_obtain: Signed in to the Chord app with Google; the app mints a short bearer (nts_…) for its own surfaces.
  location: header
  name: Google session bearer
  type: http-bearer
slug: getchord-xyz-authentication
source_filename: getchord-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://getchord.xyz/docs/concepts/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getchord.xyz/docs/concepts/authentication.md\nsources:\n- https://getchord.xyz/docs/concepts/authentication.md\n- https://getchord.xyz/docs/concepts/authentication/\n- https://getchord.xyz/developer\n- https://getchord.xyz/docs/recipes/token-page.md\ndescription: Chord uses an API key sent in the X-API-Key request header. A Google‑session bearer token can also be used for the Ask agent API,\n  but the documented primary authentication is the API key.\nschemes:\n- type: http-bearer\n  name: Google session bearer\n  evidence: POST /v1/ask — the Ask agent API (a Google session bearer also works; that is what the browser uses).\n  location: header\n  header: Authorization\n  how_to_obtain: Signed in to the Chord app with Google; the app mints a short bearer (nts_…) for its own surfaces.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other schemes are documented. 1 extracted row(s)\
  \ were dropped because their quote was not on the page.\ndocs: https://getchord.xyz/docs/concepts/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/getchord-xyz/authentication/getchord-xyz-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Trading
- Artificial Intelligence
- Cryptocurrency
---
