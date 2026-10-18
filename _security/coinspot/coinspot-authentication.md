---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coinspot-public-api-api-openapi.yml
  format: yaml
  label: CoinSpot Public API
  slug: coinspot-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-public-api-api-openapi.yml
- filename: coinspot-read-only-api-api-openapi.yml
  format: yaml
  label: CoinSpot Read Only API
  slug: coinspot-read-only-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-read-only-api-api-openapi.yml
- filename: coinspot-trading-api-api-openapi.yml
  format: yaml
  label: CoinSpot Trading API
  slug: coinspot-trading-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-trading-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coinspot Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinSpot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CoinSpot
provider_slug: coinspot
scheme_count: 2
schemes:
- description: Every POST API request carries headers key (the API key generated at https://www.coinspot.com.au/my/api) and sign (the POST data signed with the secret key using HMAC-SHA512), plus a nonce post param that must always be greater than the previous request's nonce.
  headers:
  - key
  - sign
  in: header
  name: hmac-sha512
  type: apiKey
- description: The Public API (https://www.coinspot.com.au/pubapi/v2, GET) needs no key.
  name: public
  type: none
slug: coinspot-authentication
source_filename: coinspot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CoinSpot API Authentication\ngenerated: '2026-10-13'\nmethod: searched\nsource: https://www.coinspot.com.au/v2/api\ndocs: https://www.coinspot.com.au/v2/api\nschemes:\n- name: hmac-sha512\n  type: apiKey\n  in: header\n  headers: [key, sign]\n  description: Every POST API request carries headers key (the API key generated at https://www.coinspot.com.au/my/api) and sign (the POST data signed with the secret key using HMAC-SHA512), plus a nonce post param that must always be greater than the previous request's nonce.\n- name: public\n  type: none\n  description: The Public API (https://www.coinspot.com.au/pubapi/v2, GET) needs no key.\nkey_permissions:\n- Full access and read-only API keys; withdrawal functions must be enabled via the API key options at https://www.coinspot.com.au/my/api.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/authentication/coinspot-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Australia
- Bitcoin
- Market Data
---
