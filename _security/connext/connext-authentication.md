---
api_key_in: []
api_specs:
- filename: connext-batched-intents-api-openapi.yml
  format: yaml
  label: Everclear Batched Intents API
  slug: connext-batched-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-batched-intents-api-openapi.yml
- filename: connext-configs-api-openapi.yml
  format: yaml
  label: Everclear Configs API
  slug: connext-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-configs-api-openapi.yml
- filename: connext-history-api-openapi.yml
  format: yaml
  label: Everclear History API
  slug: connext-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-history-api-openapi.yml
- filename: connext-intents-api-openapi.yml
  format: yaml
  label: Everclear Intents API
  slug: connext-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-intents-api-openapi.yml
- filename: connext-invoices-api-openapi.yml
  format: yaml
  label: Everclear Invoices API
  slug: connext-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-invoices-api-openapi.yml
- filename: connext-routes-api-openapi.yml
  format: yaml
  label: Everclear Routes API
  slug: connext-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-routes-api-openapi.yml
- filename: connext-solana-api-openapi.yml
  format: yaml
  label: Everclear Solana API
  slug: connext-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-solana-api-openapi.yml
- filename: connext-tron-api-openapi.yml
  format: yaml
  label: Everclear Tron API
  slug: connext-tron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-tron-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Connext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everclear declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Everclear
provider_slug: connext
scheme_count: 0
schemes: []
slug: connext-authentication
source_filename: connext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/connext-everclear-openapi.yml, https://docs.everclear.org/developers/api.md\nsummary: >-\n  The Everclear (\"Chimera\") API declares no authentication at all. The merged OpenAPI carries\n  no components.securitySchemes block and no security requirement on any of its 17\n  operations, and the docs never mention an API key, token, or account. Authorization in\n  Everclear is on-chain: the REST API only reads indexed protocol state and builds unsigned\n  EVM/Solana/Tron TransactionRequest objects, which the caller then signs with their own\n  wallet key and submits to the chain themselves. The signing key never touches Everclear.\nmodel: none\nschemes: []\nsecurity_requirements: []\nfindings:\n  - id: no-security-schemes\n    detail: components.securitySchemes is absent from every one of the 17 published OpenAPI documents.\n  - id: no-operation-security\n    detail: No operation declares a security[] requirement; all 17\
  \ are anonymous.\n  - id: authorization-is-on-chain\n    detail: >-\n      POST /intents, POST /solana/intents and POST /tron/intents return a TransactionRequest\n      (to/data/value/chainId or the chain equivalent) for the caller to sign locally. The\n      caller's private key is the only credential in the flow and it is never sent to the API.\n  - id: permit2-signature-in-body\n    detail: >-\n      IntentRequest accepts an optional permit2Params object (nonce, deadline, signature) —\n      an EIP-2612/Permit2 signature produced client-side. This is a token-approval signature\n      carried in the request body, not an API credential.\n  - id: no-oauth-no-oidc\n    detail: >-\n      No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any\n      host; scopes/ is therefore not applicable and is not emitted.\ndocs: https://docs.everclear.org/developers/api\ncaveat: >-\n  Unverifiable against a live host: https://api.everclear.org returned HTTP 530 on 2026-08-09,\n\
  \  so this profile is derived from the published contract only. See lifecycle/connext-lifecycle.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/authentication/connext-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Blockchain
- Cryptocurrency
- Web3
- Interoperability
- Cross Chain
- Bridging
- Settlement
- Liquidity
- Intents
- DeFi
- Chain Abstraction
- Defunct
---
