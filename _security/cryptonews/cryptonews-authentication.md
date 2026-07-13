---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: CryptoNews REST API
  slug: cryptonews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptonews/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cryptonews Authentication
name_suffix: Authentication
oauth_flows: []
overview: CryptoNews API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CryptoNews API
provider_slug: cryptonews
scheme_count: 1
schemes:
- description: API key passed as a query parameter named 'token'
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: cryptonews-authentication
source_filename: cryptonews-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: API key passed as a query parameter named 'token'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptonews/refs/heads/main/authentication/cryptonews-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- News
- Sentiment Analysis
- Bitcoin
- Market Data
- Whale Transactions
- Crypto Prices
---
