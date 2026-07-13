---
api_key_in:
- header
api_specs:
- filename: coinbase-advanced-trade-openapi.yml
  format: yaml
  label: Coinbase Advanced Trade API
  slug: advanced-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-advanced-trade-openapi.yml
- filename: coinbase-exchange-openapi.yml
  format: yaml
  label: Coinbase Exchange API
  slug: exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-exchange-openapi.yml
- filename: coinbase-prime-openapi.yml
  format: yaml
  label: Coinbase Prime API
  slug: prime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-prime-openapi.yml
- filename: coinbase-onramp-openapi.yml
  format: yaml
  label: Coinbase Onramp API
  slug: onramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-onramp-openapi.yml
- filename: coinbase-commerce-openapi.yml
  format: yaml
  label: Coinbase Commerce API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-commerce-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coinbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coinbase secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coinbase
provider_slug: coinbase
scheme_count: 4
schemes:
- description: Coinbase API key authentication using HMAC SHA-256 signatures. Requires CB-ACCESS-KEY, CB-ACCESS-SIGN, and CB-ACCESS-TIMESTAMP headers.
  in: header
  name: apiKeyAuth
  parameter: CB-ACCESS-KEY
  sources:
  - openapi/coinbase-advanced-trade-openapi.yml
  - openapi/coinbase-exchange-openapi.yml
  type: apiKey
- description: Coinbase Commerce API key for authentication. Include the key in the X-CC-Api-Key header.
  in: header
  name: apiKeyAuth
  parameter: X-CC-Api-Key
  sources:
  - openapi/coinbase-commerce-openapi.yml
  type: apiKey
- description: Bearer token authentication using a CDP API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coinbase-onramp-openapi.yml
  type: http
- description: Coinbase Prime API key authentication. Requires X-CB-ACCESS-KEY, X-CB-ACCESS-SIGNATURE, X-CB-ACCESS-TIMESTAMP, and X-CB-ACCESS-PASSPHRASE headers with HMAC SHA-256 signatures.
  in: header
  name: apiKeyAuth
  parameter: X-CB-ACCESS-KEY
  sources:
  - openapi/coinbase-prime-openapi.yml
  type: apiKey
slug: coinbase-authentication
source_filename: coinbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coinbase-advanced-trade-openapi.yml, openapi/coinbase-commerce-openapi.yml,\n  openapi/coinbase-exchange-openapi.yml, openapi/coinbase-onramp-openapi.yml, openapi/coinbase-prime-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: CB-ACCESS-KEY\n  description: Coinbase API key authentication using HMAC SHA-256 signatures. Requires CB-ACCESS-KEY,\n    CB-ACCESS-SIGN, and CB-ACCESS-TIMESTAMP headers.\n  sources:\n  - openapi/coinbase-advanced-trade-openapi.yml\n  - openapi/coinbase-exchange-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CC-Api-Key\n  description: Coinbase Commerce API key for authentication. Include the key in the X-CC-Api-Key\n    header.\n  sources:\n  - openapi/coinbase-commerce-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token\
  \ authentication using a CDP API key.\n  sources:\n  - openapi/coinbase-onramp-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CB-ACCESS-KEY\n  description: Coinbase Prime API key authentication. Requires X-CB-ACCESS-KEY, X-CB-ACCESS-SIGNATURE,\n    X-CB-ACCESS-TIMESTAMP, and X-CB-ACCESS-PASSPHRASE headers with HMAC SHA-256 signatures.\n  sources:\n  - openapi/coinbase-prime-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/authentication/coinbase-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Blockchain
- Cryptocurrency
- Custody
- Exchange
- Onramp
- Payments
- Trading
- Wallet
- Web3
---
