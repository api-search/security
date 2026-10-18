---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blofin-account-api-openapi.yml
  format: yaml
  label: BloFin Account API
  slug: blofin-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-account-api-openapi.yml
- filename: blofin-affiliate-api-openapi.yml
  format: yaml
  label: BloFin Affiliate API
  slug: blofin-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-affiliate-api-openapi.yml
- filename: blofin-asset-api-openapi.yml
  format: yaml
  label: BloFin Asset API
  slug: blofin-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-asset-api-openapi.yml
- filename: blofin-copytrading-api-openapi.yml
  format: yaml
  label: BloFin Copytrading API
  slug: blofin-copytrading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-copytrading-api-openapi.yml
- filename: blofin-market-api-openapi.yml
  format: yaml
  label: BloFin Market API
  slug: blofin-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-market-api-openapi.yml
- filename: blofin-oauth-api-openapi.yml
  format: yaml
  label: BloFin OAuth API
  slug: blofin-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-oauth-api-openapi.yml
- filename: blofin-spot-api-openapi.yml
  format: yaml
  label: BloFin Spot API
  slug: blofin-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-spot-api-openapi.yml
- filename: blofin-trade-api-openapi.yml
  format: yaml
  label: BloFin Trade API
  slug: blofin-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-trade-api-openapi.yml
- filename: blofin-user-api-openapi.yml
  format: yaml
  label: BloFin User API
  slug: blofin-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/openapi/blofin-user-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Blofin Authentication
name_suffix: Authentication
oauth_flows: []
overview: BloFin declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BloFin
provider_slug: blofin
scheme_count: 2
schemes:
- description: ACCESS-SIGN is a Base64-encoded signature over requestPath + method + timestamp + nonce + body; timestamp must be within 60s; nonce may not repeat within 60 seconds. API keys can be restricted by IP whitelist.
  headers:
  - ACCESS-KEY
  - ACCESS-SIGN
  - ACCESS-TIMESTAMP
  - ACCESS-NONCE
  - ACCESS-PASSPHRASE
  in: header
  name: HMAC-signed API key headers
  type: apiKey
- description: 'Broker API at https://oauth.blofin.com: authorization redirect, POST /oauth/token, bearer tokens for /oauth/userinfo, /oauth/apikey/create and deposit endpoints.'
  docs: https://docs.blofin.com/broker.html
  name: Broker OAuth
  type: oauth2
slug: blofin-authentication
source_filename: blofin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: BloFin authentication\ngenerated: '2026-10-13'\nmethod: searched\nsource: https://docs.blofin.com/index.html#rest-authentication\ndocs: https://docs.blofin.com/index.html#rest-authentication\nschemes:\n- type: apiKey\n  name: HMAC-signed API key headers\n  in: header\n  headers:\n  - ACCESS-KEY\n  - ACCESS-SIGN\n  - ACCESS-TIMESTAMP\n  - ACCESS-NONCE\n  - ACCESS-PASSPHRASE\n  description: ACCESS-SIGN is a Base64-encoded signature over requestPath + method + timestamp + nonce + body; timestamp must\n    be within 60s; nonce may not repeat within 60 seconds. API keys can be restricted by IP whitelist.\n- type: oauth2\n  name: Broker OAuth\n  description: 'Broker API at https://oauth.blofin.com: authorization redirect, POST /oauth/token, bearer tokens for /oauth/userinfo,\n    /oauth/apikey/create and deposit endpoints.'\n  docs: https://docs.blofin.com/broker.html\nwebsocket: Private WebSocket channels require a login event with apiKey, passphrase, timestamp, sign and nonce.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blofin/refs/heads/main/authentication/blofin-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Cryptocurrency Exchange
- Trading
- Futures
- Spot Trading
- Copy Trading
- WebSocket
---
