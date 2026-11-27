---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: FiLot Authentication
name_suffix: Authentication
oauth_flows: []
overview: FiLot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FiLot
provider_slug: filot-me
scheme_count: 1
schemes:
- notes: Public read-only MCP server. Seven tools, all read-only. No account, no login. Price answers are signed server-side with Ed25519 (compact JWS, EdDSA) whose public key is published at https://api.filot.me/functions/v1/filot-mcp/.well-known/jwks.json so clients can verify a saved answer, but the request itself carries no auth.
  scope: mcp-server
  type: none
slug: filot-me-authentication
source_filename: filot-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filot.me/ai-assistants/\nname: FiLot authentication\nsummary: >-\n  FiLot's public read-only MCP server requires no authentication. The provider\n  documents the server at mcp.filot.me/mcp (alias api.filot.me/functions/v1/filot-mcp)\n  as \"remote MCP over Streamable HTTP with JSON replies, and it needs no\n  authentication.\"\nschemes:\n  - type: none\n    scope: mcp-server\n    notes: >-\n      Public read-only MCP server. Seven tools, all read-only. No account, no login.\n      Price answers are signed server-side with Ed25519 (compact JWS, EdDSA) whose\n      public key is published at\n      https://api.filot.me/functions/v1/filot-mcp/.well-known/jwks.json so clients\n      can verify a saved answer, but the request itself carries no auth.\ndocs: https://filot.me/ai-assistants/\n"
source_yaml_url: https://artifacts.apis.io/filot-me/authentication/filot-me-authentication.yml
summary_line: 1 scheme
tags:
- Gold
- DeFi
- Solana
- Non-Custodial Wallet
- Chat-First
- Portfolio
- Liquidity Pools
- Consumer Finance
---
