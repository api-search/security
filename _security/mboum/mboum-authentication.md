---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mboum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mboum declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mboum
provider_slug: mboum
scheme_count: 2
schemes:
- description: 'Authorization: Bearer {YOUR_AUTH_KEY}. Personal Access Token issued from the Mboum account dashboard (Account -> Personal Access Tokens).'
  location: header
  name: Authorization
  scheme: bearer
  type: http
- description: apikey={YOUR_AUTH_KEY} query parameter, offered for browser and simple GET usage as an alternative to the Authorization header.
  location: query
  name: apikey
  type: apiKey
slug: mboum-authentication
source_filename: mboum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://docs.mboum.com/\nsummary: >-\n  API key (Personal Access Token) authentication. Callers pass the key either as an\n  HTTP Authorization Bearer header (\"Bearer {YOUR_AUTH_KEY}\") or, for browser/GET use,\n  as an \"apikey\" query parameter. Tokens are generated and revoked from the account\n  dashboard under Personal Access Tokens. All data endpoints require authentication.\ndocs: https://docs.mboum.com/\nschemes:\n- type: http\n  scheme: bearer\n  name: Authorization\n  location: header\n  description: >-\n    Authorization: Bearer {YOUR_AUTH_KEY}. Personal Access Token issued from the Mboum\n    account dashboard (Account -> Personal Access Tokens).\n- type: apiKey\n  name: apikey\n  location: query\n  description: >-\n    apikey={YOUR_AUTH_KEY} query parameter, offered for browser and simple GET usage\n    as an alternative to the Authorization header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mboum/refs/heads/main/authentication/mboum-authentication.yml
summary_line: 2 schemes
tags:
- Stocks
- Stock Market
- Options
- options market
- Trading
- Quotes
- Market Data
- Technical Indicators
- SEC Filings
- Insider Trading
- IPO
- Dividends
- Earnings
- Historical Data
- Screener
- Crypto
---
