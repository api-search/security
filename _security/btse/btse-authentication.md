---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: btse-account-api-openapi.yml
  format: yaml
  label: BTSE Account API
  slug: btse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-account-api-openapi.yml
- filename: btse-earn-api-openapi.yml
  format: yaml
  label: BTSE Earn API
  slug: btse-earn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-earn-api-openapi.yml
- filename: btse-markets-api-openapi.yml
  format: yaml
  label: BTSE Markets API
  slug: btse-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-markets-api-openapi.yml
- filename: btse-otc-api-openapi.yml
  format: yaml
  label: BTSE OTC API
  slug: btse-otc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-otc-api-openapi.yml
- filename: btse-trade-api-openapi.yml
  format: yaml
  label: BTSE Trade API
  slug: btse-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-api-openapi.yml
- filename: btse-trade-v3-api-openapi.yml
  format: yaml
  label: BTSE Trade V3 API
  slug: btse-trade-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-v3-api-openapi.yml
- filename: btse-trade-v4-api-openapi.yml
  format: yaml
  label: BTSE Trade V4 API
  slug: btse-trade-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-trade-v4-api-openapi.yml
- filename: btse-wallet-api-openapi.yml
  format: yaml
  label: BTSE Wallet API
  slug: btse-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/openapi/btse-wallet-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Btse Authentication
name_suffix: Authentication
oauth_flows: []
overview: BTSE secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BTSE
provider_slug: btse
scheme_count: 3
schemes:
- description: API key
  in: header
  name: api
  parameter: request-api
  sources:
  - openapi/btse-earn-openapi.yml
  - openapi/btse-futures-legacy-openapi.yml
  - openapi/btse-futures-openapi.yml
  - openapi/btse-otc-openapi.yml
  - openapi/btse-spot-legacy-openapi.yml
  - openapi/btse-spot-openapi.yml
  - openapi/btse-wallet-openapi.yml
  type: apiKey
- description: Current timestamp in milliseconds
  in: header
  name: nonce
  parameter: request-nonce
  sources:
  - openapi/btse-earn-openapi.yml
  - openapi/btse-futures-legacy-openapi.yml
  - openapi/btse-futures-openapi.yml
  - openapi/btse-otc-openapi.yml
  - openapi/btse-spot-legacy-openapi.yml
  - openapi/btse-spot-openapi.yml
  - openapi/btse-wallet-openapi.yml
  type: apiKey
- description: '`HMAC-SHA384(secret, path + nonce + body)`'
  in: header
  name: sign
  parameter: request-sign
  sources:
  - openapi/btse-earn-openapi.yml
  - openapi/btse-futures-legacy-openapi.yml
  - openapi/btse-futures-openapi.yml
  - openapi/btse-markets-openapi.yml
  - openapi/btse-otc-openapi.yml
  - openapi/btse-spot-legacy-openapi.yml
  - openapi/btse-spot-openapi.yml
  - openapi/btse-wallet-openapi.yml
  type: apiKey
slug: btse-authentication
source_filename: btse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/btse-earn-openapi.yml, openapi/btse-futures-legacy-openapi.yml, openapi/btse-futures-openapi.yml,\n  openapi/btse-markets-openapi.yml, openapi/btse-otc-openapi.yml, openapi/btse-spot-legacy-openapi.yml,\n  openapi/btse-spot-openapi.yml, openapi/btse-wallet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api\n  type: apiKey\n  in: header\n  parameter: request-api\n  description: API key\n  sources:\n  - openapi/btse-earn-openapi.yml\n  - openapi/btse-futures-legacy-openapi.yml\n  - openapi/btse-futures-openapi.yml\n  - openapi/btse-otc-openapi.yml\n  - openapi/btse-spot-legacy-openapi.yml\n  - openapi/btse-spot-openapi.yml\n  - openapi/btse-wallet-openapi.yml\n- name: nonce\n  type: apiKey\n  in: header\n  parameter: request-nonce\n  description: Current timestamp in milliseconds\n  sources:\n  - openapi/btse-earn-openapi.yml\n  - openapi/btse-futures-legacy-openapi.yml\n  - openapi/btse-futures-openapi.yml\n\
  \  - openapi/btse-otc-openapi.yml\n  - openapi/btse-spot-legacy-openapi.yml\n  - openapi/btse-spot-openapi.yml\n  - openapi/btse-wallet-openapi.yml\n- name: sign\n  type: apiKey\n  in: header\n  parameter: request-sign\n  description: '`HMAC-SHA384(secret, path + nonce + body)`'\n  sources:\n  - openapi/btse-earn-openapi.yml\n  - openapi/btse-futures-legacy-openapi.yml\n  - openapi/btse-futures-openapi.yml\n  - openapi/btse-markets-openapi.yml\n  - openapi/btse-otc-openapi.yml\n  - openapi/btse-spot-legacy-openapi.yml\n  - openapi/btse-spot-openapi.yml\n  - openapi/btse-wallet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btse/refs/heads/main/authentication/btse-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Futures
- WebSocket
---
