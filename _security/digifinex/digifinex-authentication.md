---
anonymous_access: false
api_key_in: []
api_specs:
- filename: digifinex-account-api-openapi.yml
  format: yaml
  label: DigiFinex Account API
  slug: digifinex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-account-api-openapi.yml
- filename: digifinex-copy-trading-api-openapi.yml
  format: yaml
  label: DigiFinex Copy Trading API
  slug: digifinex-copy-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-copy-trading-api-openapi.yml
- filename: digifinex-margin-api-openapi.yml
  format: yaml
  label: DigiFinex Margin API
  slug: digifinex-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-margin-api-openapi.yml
- filename: digifinex-market-data-api-openapi.yml
  format: yaml
  label: DigiFinex Market Data API
  slug: digifinex-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-market-data-api-openapi.yml
- filename: digifinex-orders-api-openapi.yml
  format: yaml
  label: DigiFinex Orders API
  slug: digifinex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-orders-api-openapi.yml
- filename: digifinex-trading-api-openapi.yml
  format: yaml
  label: DigiFinex Trading API
  slug: digifinex-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-trading-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Digifinex Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigiFinex declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: DigiFinex
provider_slug: digifinex
scheme_count: 3
schemes:
- description: User's API-KEY
  header: ACCESS-KEY
  in: header
  name: accessKey
  type: apiKey
- description: Signature of the request (query string and request body concatenated with '&', query string first), signed with the API secret
  header: ACCESS-SIGN
  in: header
  name: accessSign
  type: apiKey
- description: Timestamp in seconds; requests more than 5 seconds old are rejected unless ACCESS-RECV-WINDOW is set
  header: ACCESS-TIMESTAMP
  in: header
  name: accessTimestamp
  type: apiKey
slug: digifinex-authentication
source_filename: digifinex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: DigiFinex API Authentication\ngenerated: '2026-10-13'\nmethod: searched\nsource: https://docs.digifinex.com/en-ww/spot/v3/rest.html\ndocs: https://docs.digifinex.com/en-ww/spot/v3/rest.html\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  header: ACCESS-KEY\n  description: User's API-KEY\n- name: accessSign\n  type: apiKey\n  in: header\n  header: ACCESS-SIGN\n  description: Signature of the request (query string and request body concatenated with '&', query string first), signed with the API secret\n- name: accessTimestamp\n  type: apiKey\n  in: header\n  header: ACCESS-TIMESTAMP\n  description: Timestamp in seconds; requests more than 5 seconds old are rejected unless ACCESS-RECV-WINDOW is set\nnotes:\n- Public market-data endpoints require no signature; account, trading, transfer and wallet endpoints are signed.\n- 'Each API Key has permission property, please check the API permission'\n- Error 10007 \"IP address Unauthorized\" indicates per-key IP allowlisting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/authentication/digifinex-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- WebSocket
---
