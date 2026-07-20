---
api_key_in:
- header
api_specs:
- filename: ledgerx-market-data-asyncapi.yml
  format: yaml
  label: MIAXdx Market Data and Account API
  slug: market-data
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgerx/refs/heads/main/asyncapi/ledgerx-market-data-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ledgerx Authentication
name_suffix: Authentication
oauth_flows: []
overview: LedgerX (MIAX Derivatives Exchange) secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LedgerX (MIAX Derivatives Exchange)
provider_slug: ledgerx
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: The MIAXdx (LedgerX) APIs use JSON Web Token authentication. An API key is required for all private endpoints; public market-data endpoints such as List Contracts and List All Trades may be called unauthenticated.
  example: 'Authorization: JWT ${YOUR_API_KEY}'
  header: Authorization
  in: header
  name: JWT API Key
  scheme: bearer
  sources:
  - https://web.archive.org/web/2024/https://docs.ledgerx.com/docs/api-key
  type: http
  value_prefix: 'JWT '
- description: The WebSocket feed at wss://api.ledgerx.com/ws is authenticated by passing the API key as the token query parameter, which enables account-scoped messages (balance and position changes, and CID/MPID attribution on the caller's own action reports).
  in: query
  name: WebSocket token query parameter
  parameter: token
  sources:
  - https://web.archive.org/web/2024/https://docs.ledgerx.com/reference/connecting
  type: apiKey
slug: ledgerx-authentication
source_filename: ledgerx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://web.archive.org/web/2024/https://docs.ledgerx.com/docs/api-key\ndocs: https://docs.miaxdx.com/docs/api-key\nnote: >-\n  The live docs host (docs.miaxdx.com, formerly docs.ledgerx.com) currently returns a Cloudflare\n  error 1014 (CNAME Cross-User Banned) to external clients, so this profile was captured from the\n  provider's own archived documentation. No OpenAPI is published, so nothing here is derived from\n  a spec.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: JWT API Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  value_prefix: 'JWT '\n  example: 'Authorization: JWT ${YOUR_API_KEY}'\n  description: >-\n    The MIAXdx (LedgerX) APIs use JSON Web Token authentication. An API key is required for all\n    private endpoints; public market-data endpoints such as List Contracts and List All Trades may\n    be called unauthenticated.\n\
  \  sources:\n  - https://web.archive.org/web/2024/https://docs.ledgerx.com/docs/api-key\n- name: WebSocket token query parameter\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    The WebSocket feed at wss://api.ledgerx.com/ws is authenticated by passing the API key as the\n    token query parameter, which enables account-scoped messages (balance and position changes,\n    and CID/MPID attribution on the caller's own action reports).\n  sources:\n  - https://web.archive.org/web/2024/https://docs.ledgerx.com/reference/connecting\nkey_management:\n  console: https://app.ledgerx.com/profile/api-keys\n  create: Log in and use the API Keys page on your profile to create a key with a nickname and expiration.\n  default_expiry_days: 30\n  rotation: Keys expire by default after 30 days and must be rotated to keep connections active.\n  inheritance: All keys are assigned the same roles and permissions as the user who created them.\nroles:\n- name: Trader\n  permissions:\n\
  \  - Place orders\n  - Cancel single order\n  - Cancel all orders\n  - Submit exercise instructions\n  - View order, trade and position history\n  - View exercise instructions\n  - Create API Key\n- name: Admin\n  permissions:\n  - Cancel all orders\n  - Submit deposit notice\n  - Submit/Confirm withdrawal request\n  - Manage users and assign roles\n  - View order, trade and position history\n  - View deposit and withdrawal history\n  - View exercise instructions\n  - Create API Key\n  - Add allowlist address\n  - Remove allowlist address\n- name: Auditor\n  permissions:\n  - View order, trade and position history\n  - View deposit and withdrawal history\n  - View exercise instructions\n  - Create API Key\nrole_combinations:\n- Trader + Admin (default)\n- Trader\n- Admin\n- Auditor\nroles_source: https://web.archive.org/web/2024/https://docs.ledgerx.com/docs/roles-and-permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledgerx/refs/heads/main/authentication/ledgerx-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Enterprise
- Financial Services
- Derivatives
- Trading
- Cryptocurrency
- Bitcoin
- Exchange
- Market Data
- WebSockets
- Regulated Markets
---
