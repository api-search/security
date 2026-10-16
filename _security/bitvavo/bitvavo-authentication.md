---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bitvavo-exchange-websocket-asyncapi.yml
  format: yaml
  label: Bitvavo WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/asyncapi/bitvavo-exchange-websocket-asyncapi.yml
- filename: bitvavo-market-data-pro-asyncapi.yml
  format: yaml
  label: Bitvavo Market Data Pro WebSocket API
  slug: market-data-pro-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/asyncapi/bitvavo-market-data-pro-asyncapi.yml
- filename: bitvavo-account-api-openapi.yml
  format: yaml
  label: Bitvavo Account API
  slug: bitvavo-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-account-api-openapi.yml
- filename: bitvavo-account-management-api-openapi.yml
  format: yaml
  label: Bitvavo Account Management API
  slug: bitvavo-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-account-management-api-openapi.yml
- filename: bitvavo-market-data-api-openapi.yml
  format: yaml
  label: Bitvavo Market data API
  slug: bitvavo-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-market-data-api-openapi.yml
- filename: bitvavo-subaccounts-api-openapi.yml
  format: yaml
  label: Bitvavo Subaccounts API
  slug: bitvavo-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-subaccounts-api-openapi.yml
- filename: bitvavo-synchronization-api-openapi.yml
  format: yaml
  label: Bitvavo Synchronization API
  slug: bitvavo-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-synchronization-api-openapi.yml
- filename: bitvavo-trading-api-openapi.yml
  format: yaml
  label: Bitvavo Trading API
  slug: bitvavo-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-trading-api-openapi.yml
- filename: bitvavo-transfer-api-openapi.yml
  format: yaml
  label: Bitvavo Transfer API
  slug: bitvavo-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/openapi/bitvavo-transfer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Bitvavo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitvavo secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitvavo
provider_slug: bitvavo
scheme_count: 4
schemes:
- description: Your 64-character API key with the required [permissions](/docs/rest-api/introduction/).
  in: header
  name: Bitvavo-Access-Key
  parameter: Bitvavo-Access-Key
  sources:
  - openapi/bitvavo-exchange-rest-openapi.yml
  - openapi/bitvavo-institutional-openapi.yml
  type: apiKey
- description: A Unix timestamp in milliseconds of the time when you make the request.
  in: header
  name: Bitvavo-Access-Timestamp
  parameter: Bitvavo-Access-Timestamp
  sources:
  - openapi/bitvavo-exchange-rest-openapi.yml
  - openapi/bitvavo-institutional-openapi.yml
  type: apiKey
- description: An HMAC-SHA256 hex-encoded string of the time, HTTP method, path, and parameters used to make the request. To learn more, see [Authentication](/docs/rest-api/introduction/).
  in: header
  name: Bitvavo-Access-Signature
  parameter: Bitvavo-Access-Signature
  sources:
  - openapi/bitvavo-exchange-rest-openapi.yml
  - openapi/bitvavo-institutional-openapi.yml
  type: apiKey
- description: 'The execution timeout in milliseconds after Bitvavo-Access-Timestamp. The default value

    is 10000, the maximum value is 60000.'
  in: header
  name: Bitvavo-Access-Window
  parameter: Bitvavo-Access-Window
  sources:
  - openapi/bitvavo-exchange-rest-openapi.yml
  - openapi/bitvavo-institutional-openapi.yml
  type: apiKey
slug: bitvavo-authentication
source_filename: bitvavo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/bitvavo-exchange-rest-openapi.yml, openapi/bitvavo-institutional-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bitvavo-Access-Key\n  type: apiKey\n  in: header\n  parameter: Bitvavo-Access-Key\n  description: Your 64-character API key with the required [permissions](/docs/rest-api/introduction/).\n  sources:\n  - openapi/bitvavo-exchange-rest-openapi.yml\n  - openapi/bitvavo-institutional-openapi.yml\n- name: Bitvavo-Access-Timestamp\n  type: apiKey\n  in: header\n  parameter: Bitvavo-Access-Timestamp\n  description: A Unix timestamp in milliseconds of the time when you make the request.\n  sources:\n  - openapi/bitvavo-exchange-rest-openapi.yml\n  - openapi/bitvavo-institutional-openapi.yml\n- name: Bitvavo-Access-Signature\n  type: apiKey\n  in: header\n  parameter: Bitvavo-Access-Signature\n  description: An HMAC-SHA256 hex-encoded string of the time, HTTP method, path,\
  \ and parameters\n    used to make the request. To learn more, see [Authentication](/docs/rest-api/introduction/).\n  sources:\n  - openapi/bitvavo-exchange-rest-openapi.yml\n  - openapi/bitvavo-institutional-openapi.yml\n- name: Bitvavo-Access-Window\n  type: apiKey\n  in: header\n  parameter: Bitvavo-Access-Window\n  description: |-\n    The execution timeout in milliseconds after Bitvavo-Access-Timestamp. The default value\n    is 10000, the maximum value is 60000.\n  sources:\n  - openapi/bitvavo-exchange-rest-openapi.yml\n  - openapi/bitvavo-institutional-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitvavo/refs/heads/main/authentication/bitvavo-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Netherlands
---
