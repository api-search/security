---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitflyer-account-api-openapi.yml
  format: yaml
  label: bitFlyer Account API
  slug: bitflyer-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-account-api-openapi.yml
- filename: bitflyer-assets-api-openapi.yml
  format: yaml
  label: bitFlyer Assets API
  slug: bitflyer-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-assets-api-openapi.yml
- filename: bitflyer-chat-api-openapi.yml
  format: yaml
  label: bitFlyer Chat API
  slug: bitflyer-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-chat-api-openapi.yml
- filename: bitflyer-deposits-and-withdrawals-api-openapi.yml
  format: yaml
  label: bitFlyer Deposits and Withdrawals API
  slug: bitflyer-deposits-and-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-deposits-and-withdrawals-api-openapi.yml
- filename: bitflyer-markets-api-openapi.yml
  format: yaml
  label: bitFlyer Markets API
  slug: bitflyer-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-markets-api-openapi.yml
- filename: bitflyer-trading-api-openapi.yml
  format: yaml
  label: bitFlyer Trading API
  slug: bitflyer-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-trading-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bitflyer Authentication
name_suffix: Authentication
oauth_flows: []
overview: bitFlyer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: bitFlyer
provider_slug: bitflyer
scheme_count: 1
schemes:
- headers:
  - ACCESS-KEY
  - ACCESS-TIMESTAMP
  - ACCESS-SIGN
  in: header
  name: HMAC-signed API key
  signature: HMAC-SHA256
  type: apiKey
slug: bitflyer-authentication
source_filename: bitflyer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://lightning.bitflyer.com/docs?lang=en#authentication\nprovider: bitflyer\nsummary: >-\n  Public HTTP APIs need no key. Private APIs require an API key and secret generated on the\n  bitFlyer Lightning developer page, sent as ACCESS-KEY, ACCESS-TIMESTAMP and ACCESS-SIGN headers,\n  where ACCESS-SIGN is an HMAC-SHA256 of timestamp + HTTP method + request path + body keyed with\n  the API secret. Some withdrawal operations also document two-factor authentication.\nschemes:\n- type: apiKey\n  name: HMAC-signed API key\n  in: header\n  headers: [ACCESS-KEY, ACCESS-TIMESTAMP, ACCESS-SIGN]\n  signature: HMAC-SHA256\ndocs: https://lightning.bitflyer.com/docs?lang=en#authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/authentication/bitflyer-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Japan
---
