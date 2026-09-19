---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Itick Authentication
name_suffix: Authentication
oauth_flows: []
overview: iTick declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iTick
provider_slug: itick
scheme_count: 1
schemes:
- description: Per-account API Key issued from https://itick.org/en/dashboard. Sent as the `token` request header on REST calls and used for WebSocket authentication. In the MCP server it is supplied via the TOKEN environment variable.
  example_docs: https://docs.itick.org/en/getting-started
  id: apiKeyToken
  in: header
  name: token
  type: apiKey
slug: itick-authentication
source_filename: itick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: >-\n  https://docs.itick.org/en/getting-started and the request examples in\n  https://docs.itick.org/en/rest-api/crypto/crypto-kline.md\nsummary: >-\n  Single API-key scheme. Every REST and WebSocket request carries the account's\n  API Key in a `token` header. There is no OAuth, OIDC, or mTLS surface. The API\n  Key is issued per account from the iTick dashboard after Google/GitHub login.\nschemes:\n  - id: apiKeyToken\n    type: apiKey\n    in: header\n    name: token\n    description: >-\n      Per-account API Key issued from https://itick.org/en/dashboard. Sent as the\n      `token` request header on REST calls and used for WebSocket authentication.\n      In the MCP server it is supplied via the TOKEN environment variable.\n    example_docs: https://docs.itick.org/en/getting-started\nonboarding:\n  signup: https://itick.org/en/dashboard\n  method: OAuth login (Google or GitHub) to the dashboard, which issues the API Key.\n\
  notes:\n  - >-\n    Keys are unique per account and treated as bearer credentials - iTick's docs\n    warn against sharing them.\n  - >-\n    The free-trial environment (api-free.itick.org) uses the same header-based\n    token scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itick/refs/heads/main/authentication/itick-authentication.yml
summary_line: 1 scheme
tags:
- Financial Data
- Market Data
- Stocks
- Forex
- Crypto
- Indices
- Futures
- Fund
- Real-Time Data
- WebSocket
- FIX Protocol
- Fintech
- Quantitative Trading
- MCP Server
---
