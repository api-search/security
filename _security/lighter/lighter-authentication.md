---
api_key_in:
- header
api_specs:
- filename: lighter-account-api-openapi.yml
  format: yaml
  label: Lighter account API
  slug: lighter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-account-api-openapi.yml
- filename: lighter-announcement-api-openapi.yml
  format: yaml
  label: Lighter announcement API
  slug: lighter-announcement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-announcement-api-openapi.yml
- filename: lighter-block-api-openapi.yml
  format: yaml
  label: Lighter block API
  slug: lighter-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-block-api-openapi.yml
- filename: lighter-bridge-api-openapi.yml
  format: yaml
  label: Lighter bridge API
  slug: lighter-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-bridge-api-openapi.yml
- filename: lighter-candlestick-api-openapi.yml
  format: yaml
  label: Lighter candlestick API
  slug: lighter-candlestick-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-candlestick-api-openapi.yml
- filename: lighter-funding-api-openapi.yml
  format: yaml
  label: Lighter funding API
  slug: lighter-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-funding-api-openapi.yml
- filename: lighter-info-api-openapi.yml
  format: yaml
  label: Lighter info API
  slug: lighter-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-info-api-openapi.yml
- filename: lighter-notification-api-openapi.yml
  format: yaml
  label: Lighter notification API
  slug: lighter-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-notification-api-openapi.yml
- filename: lighter-order-api-openapi.yml
  format: yaml
  label: Lighter order API
  slug: lighter-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-order-api-openapi.yml
- filename: lighter-referral-api-openapi.yml
  format: yaml
  label: Lighter referral API
  slug: lighter-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-referral-api-openapi.yml
- filename: lighter-root-api-openapi.yml
  format: yaml
  label: Lighter root API
  slug: lighter-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-root-api-openapi.yml
- filename: lighter-tokenlist-api-openapi.yml
  format: yaml
  label: Lighter tokenlist API
  slug: lighter-tokenlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-tokenlist-api-openapi.yml
- filename: lighter-transaction-api-openapi.yml
  format: yaml
  label: Lighter transaction API
  slug: lighter-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-transaction-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lighter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lighter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lighter
provider_slug: lighter
scheme_count: 1
schemes:
- description: Auth-gated REST endpoints and WebSocket channels take an `auth` token generated from an account's API private key.
  in: header
  name: apiKey
  parameter_name: auth
  sources:
  - openapi/lighter-zklighter-openapi-original.json
  type: apiKey
slug: lighter-authentication
source_filename: lighter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lighter-zklighter-openapi-original.json\ndocs: https://apidocs.lighter.xyz/docs/api-keys\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: signed-transaction + bearer-style auth token\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: auth\n    sources: [openapi/lighter-zklighter-openapi-original.json]\n    description: >-\n      Auth-gated REST endpoints and WebSocket channels take an `auth` token generated from an\n      account's API private key.\nmodel:\n  registration:\n    description: >-\n      A Lighter account is registered by signing a message with an Ethereum wallet, which binds the\n      L1 address to a Lighter account index. Sub-accounts share the same L1 wallet and each carry\n      their own account index.\n    docs: https://docs.lighter.xyz/trading/api\n  api_keys:\n    max_per_account: 256\n    usable_index_range: '2-254'\n    reserved_indexes:\
  \ '0-3 reserved for the Lighter web and mobile interfaces'\n    lookup_index: '255 returns metadata for all API keys via the apikeys operation'\n    permissions: read and write (query auth-gated endpoints, submit transactions, process withdrawals)\n    per_key_nonce: true\n    docs: https://apidocs.lighter.xyz/docs/api-keys\n  auth_tokens:\n    - kind: canonical\n      structure: '{expiry_unix}:{account_index}:{api_key_index}:{random_hex}'\n      max_expiry: 8 hours\n      generated_by: create_auth_token_with_expiry() in the Python SDK, or the Go SDK\n    - kind: read-only\n      structure: 'ro:{account_index}:{single|all}:{expiry_unix}:{random_hex}'\n      min_expiry: 1 day\n      max_expiry: 10 years\n      max_per_account: 10\n      capabilities: read auth-gated data only; cannot sign transactions or request withdrawals\n      created_by_operation: tokens_create\n      revoked_by_operation: tokens_revoke\n      self_service_url: https://app.lighter.xyz/read-only-tokens/\n  transaction_signing:\n\
  \    description: >-\n      State-changing calls are not plain authenticated requests. The client signs a transaction body\n      with the API private key and submits it via sendTx or sendTxBatch (or the WebSocket\n      jsonapi/sendtx message). Signing is implemented in the Go SDK and wrapped by the Python\n      SignerClient.\n    operations: [sendTx, sendTxBatch]\n    docs: https://apidocs.lighter.xyz/docs/trading\n  key_restrictions:\n    maker_only_keys:\n      description: >-\n        Premium accounts may mark up to 251 keys per account index as maker-only, restricting them\n        to post-only (ALO) orders, modifies on ALO orders, and cancels, in exchange for a lower\n        latency execution path. Indexes 0-3 cannot be maker-only; changes have a one-hour cooldown.\n      operations: [getMakerOnlyApiKeys, setMakerOnlyApiKeys]\n  l1_signature_required_for:\n    - Fast Withdrawals to a different L1 address\n    - Transfers to another L1 address\n    - Associating a newly generated\
  \ API key with an account (ChangePubKey)\n  scopes:\n    supported: false\n    evidence: >-\n      Error 61004 \"custom scopes for api tokens are not supported yet\" - Lighter has no OAuth or\n      scope surface, so no scopes/ artifact is produced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/authentication/lighter-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Trading
- Cryptocurrency
- Decentralized Finance
- Perpetual Futures
- Exchange
- Blockchain
- Zero Knowledge
- Market Data
- WebSockets
---
