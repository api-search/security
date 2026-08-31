---
api_key_in:
- header
api_specs:
- filename: alpaca-trading-api-openapi.yml
  format: yaml
  label: Alpaca Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-trading-api-openapi.yml
- filename: alpaca-oauth-api-openapi.yml
  format: yaml
  label: Alpaca OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-oauth-api-openapi.yml
- filename: alpaca-accounts-api-openapi.yml
  format: yaml
  label: Alpaca Accounts API
  slug: alpaca-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-accounts-api-openapi.yml
- filename: alpaca-assets-api-openapi.yml
  format: yaml
  label: Alpaca Assets API
  slug: alpaca-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-assets-api-openapi.yml
- filename: alpaca-calendar-api-openapi.yml
  format: yaml
  label: Alpaca Calendar API
  slug: alpaca-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-calendar-api-openapi.yml
- filename: alpaca-clock-api-openapi.yml
  format: yaml
  label: Alpaca Clock API
  slug: alpaca-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-clock-api-openapi.yml
- filename: alpaca-corporate-actions-api-openapi.yml
  format: yaml
  label: Alpaca Corporate Actions API
  slug: alpaca-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-corporate-actions-api-openapi.yml
- filename: alpaca-crypto-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Crypto Pricing Data API API
  slug: alpaca-crypto-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-crypto-pricing-data-api-api-openapi.yml
- filename: alpaca-documents-api-openapi.yml
  format: yaml
  label: Alpaca Documents API
  slug: alpaca-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-documents-api-openapi.yml
- filename: alpaca-events-api-openapi.yml
  format: yaml
  label: Alpaca Events API
  slug: alpaca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-events-api-openapi.yml
- filename: alpaca-funding-api-openapi.yml
  format: yaml
  label: Alpaca Funding API
  slug: alpaca-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-funding-api-openapi.yml
- filename: alpaca-journals-api-openapi.yml
  format: yaml
  label: Alpaca Journals API
  slug: alpaca-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-journals-api-openapi.yml
- filename: alpaca-logo-api-openapi.yml
  format: yaml
  label: Alpaca Logo API
  slug: alpaca-logo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-logo-api-openapi.yml
- filename: alpaca-news-api-openapi.yml
  format: yaml
  label: Alpaca News API
  slug: alpaca-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-news-api-openapi.yml
- filename: alpaca-screener-api-openapi.yml
  format: yaml
  label: Alpaca Screener API
  slug: alpaca-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-screener-api-openapi.yml
- filename: alpaca-stock-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Stock Pricing Data API API
  slug: alpaca-stock-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-stock-pricing-data-api-api-openapi.yml
- filename: alpaca-watchlist-api-openapi.yml
  format: yaml
  label: Alpaca Watchlist API
  slug: alpaca-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-watchlist-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alpaca Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Alpaca secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Alpaca
provider_slug: alpaca
scheme_count: 5
schemes:
- name: BasicAuth
  note: Broker API — API key as username, API secret as password.
  scheme: basic
  sources:
  - openapi/alpaca-broker-api-openapi.yml
  type: http
- in: header
  name: API_Key
  parameter: APCA-API-KEY-ID
  sources:
  - openapi/alpaca-data-api-openapi.yml
  - openapi/alpaca-oauth-api-openapi.yml
  - openapi/alpaca-trading-api-openapi.yml
  type: apiKey
- in: header
  name: API_Secret
  parameter: APCA-API-SECRET-KEY
  sources:
  - openapi/alpaca-data-api-openapi.yml
  - openapi/alpaca-oauth-api-openapi.yml
  - openapi/alpaca-trading-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://app.alpaca.markets/oauth/authorize
    flow: authorizationCode
    scopes:
    - account:write
    - trading
    - data
    tokenUrl: https://api.alpaca.markets/oauth/token
  name: ConnectOAuth2
  note: Alpaca Connect — third-party apps act for Alpaca users on the Trading and Market Data APIs with a Bearer access token; read-only access is the default when no scope is requested. Not declared in the harvested OpenAPI; documented at docs.alpaca.markets. See scopes/alpaca-scopes.yml.
  sources:
  - https://docs.alpaca.markets/docs/using-oauth2-and-trading-api
  type: oauth2
- flows:
  - authorizationUrl: https://authx.alpaca.markets/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authx.alpaca.markets/v1/oauth2/token
  name: authx (Broker MCP)
  note: Authorization server fronting the hosted Broker MCP Server (PKCE S256; also client_credentials, jwt-bearer, refresh_token grants). Metadata saved in well-known/alpaca-authx-oauth-authorization-server.json.
  sources:
  - https://authx.alpaca.markets/v1/.well-known/oauth-authorization-server
  type: oauth2
slug: alpaca-authentication
source_filename: alpaca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/alpaca-broker-api-openapi.yml, openapi/alpaca-data-api-openapi.yml, openapi/alpaca-oauth-api-openapi.yml,\n  openapi/alpaca-trading-api-openapi.yml\ndocs: https://docs.alpaca.markets/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  note: Broker API — API key as username, API secret as password.\n  sources:\n  - openapi/alpaca-broker-api-openapi.yml\n- name: API_Key\n  type: apiKey\n  in: header\n  parameter: APCA-API-KEY-ID\n  sources:\n  - openapi/alpaca-data-api-openapi.yml\n  - openapi/alpaca-oauth-api-openapi.yml\n  - openapi/alpaca-trading-api-openapi.yml\n- name: API_Secret\n  type: apiKey\n  in: header\n  parameter: APCA-API-SECRET-KEY\n  sources:\n  - openapi/alpaca-data-api-openapi.yml\n  - openapi/alpaca-oauth-api-openapi.yml\n  - openapi/alpaca-trading-api-openapi.yml\n\
  - name: ConnectOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.alpaca.markets/oauth/authorize\n    tokenUrl: https://api.alpaca.markets/oauth/token\n    scopes: [account:write, trading, data]\n  note: >-\n    Alpaca Connect — third-party apps act for Alpaca users on the Trading and Market Data APIs\n    with a Bearer access token; read-only access is the default when no scope is requested.\n    Not declared in the harvested OpenAPI; documented at docs.alpaca.markets. See\n    scopes/alpaca-scopes.yml.\n  sources:\n  - https://docs.alpaca.markets/docs/using-oauth2-and-trading-api\n- name: authx (Broker MCP)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authx.alpaca.markets/v1/oauth2/authorize\n    tokenUrl: https://authx.alpaca.markets/v1/oauth2/token\n  note: >-\n    Authorization server fronting the hosted Broker MCP Server (PKCE S256; also client_credentials,\n    jwt-bearer, refresh_token grants).\
  \ Metadata saved in\n    well-known/alpaca-authx-oauth-authorization-server.json.\n  sources:\n  - https://authx.alpaca.markets/v1/.well-known/oauth-authorization-server\npaper_trading:\n  note: Paper environment uses the same schemes with separate keys against https://paper-api.alpaca.markets.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/authentication/alpaca-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Fintech
- Trading
- Stocks
- Crypto
- Brokerage
- Market Data
- Options
---
