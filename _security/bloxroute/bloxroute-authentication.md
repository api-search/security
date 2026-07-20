---
api_key_in:
- header
api_specs:
- filename: bloxroute-streams-asyncapi.yml
  format: yaml
  label: bloXroute Solana Trader API
  slug: bloxroute-solana-trader-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloxroute/refs/heads/main/asyncapi/bloxroute-streams-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bloxroute Authentication
name_suffix: Authentication
oauth_flows: []
overview: bloXroute secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: bloXroute
provider_slug: bloxroute
scheme_count: 1
schemes:
- description: All BDN / Cloud-API / Trader-API requests require an Authorization header whose value is the account secret retrieved from the bloXroute Account Portal (Account Details). The same header authorizes transaction submission, stream subscriptions, and account-usage checks.
  in: header
  name: AuthorizationHeader
  obtain: https://portal.bloxroute.com/
  parameter_name: Authorization
  sources:
  - https://docs.bloxroute.com/getting-started/authorization-headers
  type: apiKey
slug: bloxroute-authentication
source_filename: bloxroute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bloxroute.com/getting-started/authorization-headers\ndocs: https://docs.bloxroute.com/getting-started/authorization-headers\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: AuthorizationHeader\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: >-\n      All BDN / Cloud-API / Trader-API requests require an Authorization header\n      whose value is the account secret retrieved from the bloXroute Account\n      Portal (Account Details). The same header authorizes transaction\n      submission, stream subscriptions, and account-usage checks.\n    obtain: https://portal.bloxroute.com/\n    sources:\n      - https://docs.bloxroute.com/getting-started/authorization-headers\nnotes:\n  - The Solana Trader API additionally supports client-certificate (mTLS) auth on the QUIC transport (solana-trader-quic-client-rust).\n  - BDN gateways use certificate-based\
  \ authentication (per-account SSL certs) documented under each chain's Gateway > Authentication & Certificates.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloxroute/refs/heads/main/authentication/bloxroute-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Blockchain
- Trading
- MEV
- Solana
- Ethereum
- Low Latency
- Streaming
- Infrastructure
---
