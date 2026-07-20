---
api_key_in:
- header
auth_types:
- http-bearer
- apiKey
- wallet
description: ''
kind: authentication
layout: security
method: searched
name: Bitbond Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitbond secures its APIs with http-bearer, apiKey, and wallet across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitbond
provider_slug: bitbond
scheme_count: 4
schemes:
- api: Bitbond Offering Manager API
  applies_to: Offering Manager public investor API (POST /orders, order/portfolio reads, checkout-intent, payments/checkout-session, payments/checkout-pay, kyc/init, kyc/status, investor/profile, investor GDPR export/erase).
  bearer_format: Privy ID token (JWT)
  header: Authorization
  in: header
  name: privy-bearer
  scheme: bearer
  sources:
  - https://om.bitbond.com/api/docs
  type: http
- alt: session JWT
  api: Bitbond Offering Manager API
  applies_to: Offering Manager issuer-management API under /api/issuer/* (audit-logs, order wallet exports, team management). Authenticated with an issuer API key or a logged-in session JWT.
  in: header
  name: issuer-api-key
  sources:
  - https://om.bitbond.com/api/docs
  type: apiKey
- api: Bitbond Offering Manager API
  applies_to: 'A subset of Offering Manager public endpoints require no auth: GET /offerings/:slug, GET /documents/:docId/download, GET /token-info, GET /payments/checkout-config, and the activation-email unsubscribe endpoints.'
  name: public-unauthenticated
  type: none
- api: Bitbond Token Tool API
  applies_to: Token Tool self-serve app authenticates by connecting a web3 wallet at tokentool.bitbond.com; contract-level actions are signed by the connected wallet rather than an API credential.
  name: wallet-connect
  type: wallet
slug: bitbond-authentication
source_filename: bitbond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bitbond.com/asset-tokenization-suite/offering-manager/intro-offering-manager\ndocs: https://om.bitbond.com/api/docs\nsummary:\n  types: [http-bearer, apiKey, wallet]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: privy-bearer\n  type: http\n  scheme: bearer\n  bearer_format: Privy ID token (JWT)\n  in: header\n  header: Authorization\n  applies_to: >-\n    Offering Manager public investor API (POST /orders, order/portfolio reads,\n    checkout-intent, payments/checkout-session, payments/checkout-pay, kyc/init,\n    kyc/status, investor/profile, investor GDPR export/erase).\n  api: Bitbond Offering Manager API\n  sources: [https://om.bitbond.com/api/docs]\n- name: issuer-api-key\n  type: apiKey\n  in: header\n  alt: session JWT\n  applies_to: >-\n    Offering Manager issuer-management API under /api/issuer/* (audit-logs, order\n    wallet exports, team management). Authenticated with an issuer API\
  \ key or a\n    logged-in session JWT.\n  api: Bitbond Offering Manager API\n  sources: [https://om.bitbond.com/api/docs]\n- name: public-unauthenticated\n  type: none\n  applies_to: >-\n    A subset of Offering Manager public endpoints require no auth: GET\n    /offerings/:slug, GET /documents/:docId/download, GET /token-info, GET\n    /payments/checkout-config, and the activation-email unsubscribe endpoints.\n  api: Bitbond Offering Manager API\n- name: wallet-connect\n  type: wallet\n  applies_to: >-\n    Token Tool self-serve app authenticates by connecting a web3 wallet at\n    tokentool.bitbond.com; contract-level actions are signed by the connected\n    wallet rather than an API credential.\n  api: Bitbond Token Tool API\nnotes: >-\n  No OpenAPI spec is publicly downloadable (the Scalar reference at\n  om.bitbond.com/api/docs and its JSON are Cloudflare-gated), so this profile is\n  captured from the published GitBook API documentation rather than derived from\n  a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbond/refs/heads/main/authentication/bitbond-authentication.yml
summary_line: http-bearer/apiKey/wallet · 4 schemes
tags:
- Company
- Tokenization
- Blockchain
- Digital Assets
- Smart Contracts
- Web3
- Securities
- Payments
- MCP
---
