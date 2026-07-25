---
api_key_in:
- header
api_specs:
- filename: hifi-account-api-openapi.yml
  format: yaml
  label: Hifi Account API
  slug: hifi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-account-api-openapi.yml
- filename: hifi-common-api-openapi.yml
  format: yaml
  label: Hifi Common API
  slug: hifi-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-common-api-openapi.yml
- filename: hifi-cross-chain-bridge-api-openapi.yml
  format: yaml
  label: Hifi Cross-Chain Bridge API
  slug: hifi-cross-chain-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-cross-chain-bridge-api-openapi.yml
- filename: hifi-crypto-transfer-api-openapi.yml
  format: yaml
  label: Hifi Crypto Transfer API
  slug: hifi-crypto-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-crypto-transfer-api-openapi.yml
- filename: hifi-file-api-openapi.yml
  format: yaml
  label: Hifi File API
  slug: hifi-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-file-api-openapi.yml
- filename: hifi-kyc-api-openapi.yml
  format: yaml
  label: Hifi Kyc API
  slug: hifi-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-kyc-api-openapi.yml
- filename: hifi-offramp-api-openapi.yml
  format: yaml
  label: Hifi Offramp API
  slug: hifi-offramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-offramp-api-openapi.yml
- filename: hifi-onramp-api-openapi.yml
  format: yaml
  label: Hifi Onramp API
  slug: hifi-onramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-onramp-api-openapi.yml
- filename: hifi-reporting-api-openapi.yml
  format: yaml
  label: Hifi Reporting API
  slug: hifi-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-reporting-api-openapi.yml
- filename: hifi-settlement-rules-api-openapi.yml
  format: yaml
  label: Hifi Settlement Rules API
  slug: hifi-settlement-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-settlement-rules-api-openapi.yml
- filename: hifi-token-swap-api-openapi.yml
  format: yaml
  label: Hifi Token Swap API
  slug: hifi-token-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-token-swap-api-openapi.yml
- filename: hifi-transfer-approvals-api-openapi.yml
  format: yaml
  label: Hifi Transfer Approvals API
  slug: hifi-transfer-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-transfer-approvals-api-openapi.yml
- filename: hifi-user-api-openapi.yml
  format: yaml
  label: Hifi User API
  slug: hifi-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-user-api-openapi.yml
- filename: hifi-virtual-account-api-openapi.yml
  format: yaml
  label: Hifi Virtual Account API
  slug: hifi-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-virtual-account-api-openapi.yml
- filename: hifi-wallet-api-openapi.yml
  format: yaml
  label: Hifi Wallet API
  slug: hifi-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hifi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hifi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hifi
provider_slug: hifi
scheme_count: 1
schemes:
- bearerFormat: JWT
  header_name: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hifi-openapi-original.json
  type: http
slug: hifi-authentication
source_filename: hifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hifi-openapi-original.json\ndocs: https://docs.hifi.com/api/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  scheme: All requests are authenticated with a bearer API key sent in the\n    Authorization header over HTTPS/TLS. Keys are created in the Hifi Dashboard\n    under Developer > API Keys and shown only once at creation.\nnotes:\n- Header format is \"Authorization: Bearer [example key]\".\n- Separate keys per environment; sandbox keys must never be used in production\n  and vice versa. There is no documented test/live key prefix.\n- Webhook callbacks are themselves signed as an RS256 JWT in the Authorization\n  header, verified with the per-endpoint webhook public key.\n- Recommended rotation is annual, or immediately on suspected compromise.\nenvironments:\n- name: sandbox\n  base_url: https://sandbox.hifibridge.com\n- name: production\n  base_url: https://production.hifibridge.com\n\
  schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header_name: Authorization\n  sources:\n  - openapi/hifi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/authentication/hifi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Stablecoins
- Payments
- Money Movement
- On-Ramp
- Off-Ramp
- Crypto
- Fintech
- KYC
- Virtual Accounts
- Cross-Chain
- Financial Infrastructure
---
