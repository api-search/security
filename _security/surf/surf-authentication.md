---
api_key_in:
- header
api_specs:
- filename: surf-dex-api-openapi.yml
  format: yaml
  label: Surf DEX API
  slug: surf-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-dex-api-openapi.yml
- filename: surf-exchange-api-openapi.yml
  format: yaml
  label: Surf Exchange API
  slug: surf-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-exchange-api-openapi.yml
- filename: surf-fund-api-openapi.yml
  format: yaml
  label: Surf Fund API
  slug: surf-fund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-fund-api-openapi.yml
- filename: surf-hyperliquid-api-openapi.yml
  format: yaml
  label: Surf Hyperliquid API
  slug: surf-hyperliquid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-hyperliquid-api-openapi.yml
- filename: surf-market-api-openapi.yml
  format: yaml
  label: Surf Market API
  slug: surf-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-market-api-openapi.yml
- filename: surf-news-api-openapi.yml
  format: yaml
  label: Surf News API
  slug: surf-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-news-api-openapi.yml
- filename: surf-onchain-api-openapi.yml
  format: yaml
  label: Surf Onchain API
  slug: surf-onchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-onchain-api-openapi.yml
- filename: surf-prediction-market-api-openapi.yml
  format: yaml
  label: Surf Prediction Market API
  slug: surf-prediction-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-prediction-market-api-openapi.yml
- filename: surf-project-api-openapi.yml
  format: yaml
  label: Surf Project API
  slug: surf-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-project-api-openapi.yml
- filename: surf-search-api-openapi.yml
  format: yaml
  label: Surf Search API
  slug: surf-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-search-api-openapi.yml
- filename: surf-signal-api-openapi.yml
  format: yaml
  label: Surf Signal API
  slug: surf-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-signal-api-openapi.yml
- filename: surf-social-api-openapi.yml
  format: yaml
  label: Surf Social API
  slug: surf-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-social-api-openapi.yml
- filename: surf-token-api-openapi.yml
  format: yaml
  label: Surf Token API
  slug: surf-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-token-api-openapi.yml
- filename: surf-wallet-api-openapi.yml
  format: yaml
  label: Surf Wallet API
  slug: surf-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-wallet-api-openapi.yml
- filename: surf-web-api-openapi.yml
  format: yaml
  label: Surf Web API
  slug: surf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-web-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Surf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surf secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Surf
provider_slug: surf
scheme_count: 3
schemes:
- audience: public
  bearerFormat: JWT
  header: 'Authorization: Bearer sk-...'
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/surf-openapi-original.json
  type: http
- audience: internal
  in: header
  name: AdminToken
  parameter: X-Admin-Token
  sources:
  - openapi/surf-openapi-original.json
  type: apiKey
- audience: internal
  in: header
  name: InternalKey
  parameter: X-Internal-Key
  sources:
  - openapi/surf-openapi-original.json
  type: apiKey
slug: surf-authentication
source_filename: surf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/surf-openapi-original.json\ndocs: https://agents.asksurf.ai/docs/cli/introduction\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  public_scheme: bearer\nnotes: >-\n  Public access uses a single Bearer API key (keys are prefixed `sk-`), passed in the\n  `Authorization: Bearer $SURF_API_KEY` header, generated from the dashboard at\n  agents.asksurf.ai. The OpenAPI also declares AdminToken (X-Admin-Token) and InternalKey\n  (X-Internal-Key) apiKey schemes that are internal/admin-only and not for public consumers.\n  The gateway also serves 30 free credits per day per IP with no key at all.\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  audience: public\n  header: 'Authorization: Bearer sk-...'\n  sources:\n  - openapi/surf-openapi-original.json\n- name: AdminToken\n  type: apiKey\n  in: header\n  parameter: X-Admin-Token\n  audience: internal\n  sources:\n\
  \  - openapi/surf-openapi-original.json\n- name: InternalKey\n  type: apiKey\n  in: header\n  parameter: X-Internal-Key\n  audience: internal\n  sources:\n  - openapi/surf-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/authentication/surf-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- Market Data
- On-Chain Analytics
- Wallet Intelligence
- Artificial Intelligence
- DeFi
- Prediction Markets
- Developer API
---
