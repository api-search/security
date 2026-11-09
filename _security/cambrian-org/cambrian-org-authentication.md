---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Cambrian Network APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cambrian Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cambrian Network declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cambrian Network
provider_slug: cambrian-org
scheme_count: 2
schemes:
- evidence: 'Authentication: X-API-Key header'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: agents like Claude Code, Codex, Hermes, and OpenClaw can access the Cambrian API without an API key. All Cambrian endpoints and the Cambrian CLI support pay-per-request via the x402 payment protocol (v2) with USDC on Base.
  how_to_obtain: Pay $0.05 USDC per request using a wallet that signs the payment authorization
  name: x402
  type: other
slug: cambrian-org-authentication
source_filename: cambrian-org-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cambrian.org/guides/x402-use-the-cambrian-api-without-an-api-key-ms8xy1mi
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cambrian.org/guides/x402-use-the-cambrian-api-without-an-api-key-ms8xy1mi\nsources:\n- https://docs.cambrian.org/guides/x402-use-the-cambrian-api-without-an-api-key-ms8xy1mi\n- https://docs.cambrian.org/deep42/social-data/token-analysis\n- https://docs.cambrian.org/evm/tokens\n- https://docs.cambrian.org/solana/holder-token-balances\ndescription: Authentication methods for Cambrian Network APIs\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Authentication: X-API-Key header'\n  location: header\n  header: X-API-Key\n- type: other\n  name: x402\n  evidence: agents like Claude Code, Codex, Hermes, and OpenClaw can access the Cambrian API without an API key. All Cambrian endpoints and the\n    Cambrian CLI support pay-per-request via the x402 payment protocol (v2) with USDC on Base.\n  how_to_obtain: Pay $0.05 USDC per request using a wallet that signs the payment\
  \ authorization\ndocs: https://docs.cambrian.org/guides/x402-use-the-cambrian-api-without-an-api-key-ms8xy1mi\n"
source_yaml_url: https://artifacts.apis.io/cambrian-org/authentication/cambrian-org-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Digital Assets
- On-Chain Data
- Market Intelligence
- Cryptocurrency
---
