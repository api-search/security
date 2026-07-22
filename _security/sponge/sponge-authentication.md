---
api_key_in: []
api_specs:
- filename: sponge-openapi-original.json
  format: json
  label: Sponge Wallet API
  slug: sponge-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/openapi/sponge-openapi-original.json
auth_types:
- http
- oauth2
- openIdConnect
description: Sponge's public Wallet API authenticates with a per-agent bearer API key. A browser device flow issues agent credentials interactively; agent keys are used non-interactively for servers/CI. Separately, an OAuth 2.0 / OIDC authorization server (S256 PKCE, dynamic client registration) fronts the hosted MCP servers for connectors that support OAuth.
kind: authentication
layout: security
method: searched
name: Sponge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sponge secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sponge
provider_slug: sponge
scheme_count: 4
schemes:
- bearerFormat: API Key
  env: SPONGE_API_KEY
  key_prefixes:
  - sponge_live_
  - sponge_test_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sponge-openapi-original.json
  - https://docs.paysponge.com/wallet/ai-agents.md
  type: http
- description: SpongeWallet.connect() starts a browser-based device flow when no local credentials exist; credentials cached at ~/.spongewallet/credentials.json with owner-only permissions.
  name: DeviceFlow
  sources:
  - https://docs.paysponge.com/wallet/ai-agents.md
  type: oauth2-device
- authorization_url: https://api.wallet.paysponge.com/oauth/authorize
  description: OAuth 2.0 authorization-code flow (S256 PKCE, dynamic client registration) fronting the hosted MCP servers.
  name: OAuth2
  scopes_ref: scopes/sponge-scopes.yml
  sources:
  - well-known/sponge-openid-configuration.json
  token_url: https://api.wallet.paysponge.com/oauth/token
  type: oauth2
- description: Sign-In With Ethereum (EIP-4361) signatures for endpoints that require them (POST /api/siwe/generate).
  name: SIWE
  sources:
  - https://sponge.md
  type: eip-4361
slug: sponge-authentication
source_filename: sponge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sponge-openapi-original.json\ndocs: https://docs.paysponge.com/wallet/ai-agents.md\ndescription: >-\n  Sponge's public Wallet API authenticates with a per-agent bearer API key. A\n  browser device flow issues agent credentials interactively; agent keys are used\n  non-interactively for servers/CI. Separately, an OAuth 2.0 / OIDC authorization\n  server (S256 PKCE, dynamic client registration) fronts the hosted MCP servers\n  for connectors that support OAuth.\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_prefixes: [sponge_live_, sponge_test_]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  key_prefixes: [sponge_live_, sponge_test_]\n  env: SPONGE_API_KEY\n  sources:\n  - openapi/sponge-openapi-original.json\n  - https://docs.paysponge.com/wallet/ai-agents.md\n- name: DeviceFlow\n  type: oauth2-device\n  description:\
  \ SpongeWallet.connect() starts a browser-based device flow when no local credentials exist; credentials cached at ~/.spongewallet/credentials.json with owner-only permissions.\n  sources:\n  - https://docs.paysponge.com/wallet/ai-agents.md\n- name: OAuth2\n  type: oauth2\n  description: OAuth 2.0 authorization-code flow (S256 PKCE, dynamic client registration) fronting the hosted MCP servers.\n  authorization_url: https://api.wallet.paysponge.com/oauth/authorize\n  token_url: https://api.wallet.paysponge.com/oauth/token\n  scopes_ref: scopes/sponge-scopes.yml\n  sources:\n  - well-known/sponge-openid-configuration.json\n- name: SIWE\n  type: eip-4361\n  description: Sign-In With Ethereum (EIP-4361) signatures for endpoints that require them (POST /api/siwe/generate).\n  sources:\n  - https://sponge.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/authentication/sponge-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Agent Payments
- AI Agents
- Wallets
- Cryptocurrency
- Payments
- Stablecoins
- x402
- MPP
- Financial Infrastructure
- MCP
- Fintech
- Cards
- Onramp
---
