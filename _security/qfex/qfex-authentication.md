---
api_key_in:
- header
api_specs:
- filename: qfex-openapi-original.yml
  format: yaml
  label: QFEX REST API
  slug: qfex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/openapi/qfex-openapi-original.yml
- filename: qfex-mds-asyncapi.yml
  format: yaml
  label: QFEX Market Data WebSocket (MDS)
  slug: qfex-market-data-websocket-mds
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/asyncapi/qfex-mds-asyncapi.yml
- filename: qfex-trade-asyncapi.yml
  format: yaml
  label: QFEX Trade WebSocket
  slug: qfex-trade-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/asyncapi/qfex-trade-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qfex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qfex secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qfex
provider_slug: qfex
scheme_count: 4
schemes:
- description: HMAC-SHA256 signature (hex-encoded).
  in: header
  name: HMACSignature
  parameter: x-qfex-hmac-signature
  sources:
  - openapi/qfex-openapi-original.yml
  type: apiKey
- description: Unique request nonce (hex encoded, max 100 characters).
  in: header
  name: Nonce
  parameter: x-qfex-nonce
  sources:
  - openapi/qfex-openapi-original.yml
  type: apiKey
- description: 'QFEX API Authentication requires these headers:


    - **x-qfex-public-key**: Your public API key

    - **x-qfex-hmac-signature**: HMAC signature of the request (hex encoded)

    - **x-qfex-nonce**: Unique nonce for the request (hex encoded, max 100 characters)

    - **x-qfex-timestamp**: Unix timestamp of the request


    These four are required. Optionally send **x-qfex-requested-account-id** (UUID) to act as a sub'
  in: header
  name: PublicKey
  parameter: x-qfex-public-key
  sources:
  - openapi/qfex-openapi-original.yml
  type: apiKey
- description: Unix timestamp (seconds since epoch).
  in: header
  name: Timestamp
  parameter: x-qfex-timestamp
  sources:
  - openapi/qfex-openapi-original.yml
  type: apiKey
slug: qfex-authentication
source_filename: qfex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qfex-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HMACSignature\n  type: apiKey\n  in: header\n  parameter: x-qfex-hmac-signature\n  description: HMAC-SHA256 signature (hex-encoded).\n  sources:\n  - openapi/qfex-openapi-original.yml\n- name: Nonce\n  type: apiKey\n  in: header\n  parameter: x-qfex-nonce\n  description: Unique request nonce (hex encoded, max 100 characters).\n  sources:\n  - openapi/qfex-openapi-original.yml\n- name: PublicKey\n  type: apiKey\n  in: header\n  parameter: x-qfex-public-key\n  description: |-\n    QFEX API Authentication requires these headers:\n\n    - **x-qfex-public-key**: Your public API key\n    - **x-qfex-hmac-signature**: HMAC signature of the request (hex encoded)\n    - **x-qfex-nonce**: Unique nonce for the request (hex encoded, max 100 characters)\n    - **x-qfex-timestamp**: Unix timestamp of the request\n\n    These four\
  \ are required. Optionally send **x-qfex-requested-account-id** (UUID) to act as a sub\n  sources:\n  - openapi/qfex-openapi-original.yml\n- name: Timestamp\n  type: apiKey\n  in: header\n  parameter: x-qfex-timestamp\n  description: Unix timestamp (seconds since epoch).\n  sources:\n  - openapi/qfex-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/authentication/qfex-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Trading
- Exchange
- Perpetual Futures
- Market Data
- WebSocket
- FX
- Commodities
- Equities
- Financial Services
- CLI
- Fintech
- Real-time
---
