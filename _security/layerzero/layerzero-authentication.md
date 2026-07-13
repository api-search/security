---
api_key_in:
- header
api_specs:
- filename: scan-mainnet.json
  format: json
  label: LayerZero Scan API
  slug: layerzero-scan-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/scan-mainnet.json
- filename: scan-testnet.json
  format: json
  label: LayerZero Scan API (Testnet)
  slug: layerzero-scan-api-testnet
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/scan-testnet.json
- filename: vt-api.json
  format: json
  label: LayerZero Value Transfer API
  slug: layerzero-value-transfer-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/vt-api.json
- filename: oft-mainnet.json
  format: json
  label: LayerZero OFT Transfer API
  slug: layerzero-oft-transfer-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/oft-mainnet.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Layerzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: LayerZero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LayerZero
provider_slug: layerzero
scheme_count: 1
schemes:
- description: API key for authenticating requests. Required for /quotes, /build-user-steps, /submit-signature, and /status endpoints.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/vt-api.json
  type: apiKey
slug: layerzero-authentication
source_filename: layerzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vt-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authenticating requests. Required for /quotes, /build-user-steps,\n    /submit-signature, and /status endpoints.\n  sources:\n  - openapi/vt-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layerzero/refs/heads/main/authentication/layerzero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cross-Chain
- Omnichain
- Interoperability
- Web3
- DeFi
- Messaging
- Token Transfers
---
