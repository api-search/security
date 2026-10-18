---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: quant-api-keys-api-openapi.yml
  format: yaml
  label: Quant Network API Keys API
  slug: quant-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-api-keys-api-openapi.yml
- filename: quant-contracts-api-openapi.yml
  format: yaml
  label: Quant Network Contracts API
  slug: quant-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-contracts-api-openapi.yml
- filename: quant-deposits-api-openapi.yml
  format: yaml
  label: Quant Network Deposits API
  slug: quant-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-deposits-api-openapi.yml
- filename: quant-flow-query-api-openapi.yml
  format: yaml
  label: Quant Network Flow Query API
  slug: quant-flow-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-query-api-openapi.yml
- filename: quant-flow-registry-api-openapi.yml
  format: yaml
  label: Quant Network Flow Registry API
  slug: quant-flow-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-registry-api-openapi.yml
- filename: quant-flow-sessions-api-openapi.yml
  format: yaml
  label: Quant Network Flow Sessions API
  slug: quant-flow-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-sessions-api-openapi.yml
- filename: quant-flow-webhooks-api-openapi.yml
  format: yaml
  label: Quant Network Flow Webhooks API
  slug: quant-flow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-webhooks-api-openapi.yml
- filename: quant-health-api-openapi.yml
  format: yaml
  label: Quant Network Health API
  slug: quant-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-health-api-openapi.yml
- filename: quant-networks-api-openapi.yml
  format: yaml
  label: Quant Network Networks API
  slug: quant-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-networks-api-openapi.yml
- filename: quant-nodes-api-openapi.yml
  format: yaml
  label: Quant Network Nodes API
  slug: quant-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-nodes-api-openapi.yml
- filename: quant-observability-api-openapi.yml
  format: yaml
  label: Quant Network Observability API
  slug: quant-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-observability-api-openapi.yml
- filename: quant-rpc-api-openapi.yml
  format: yaml
  label: Quant Network RPC API
  slug: quant-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-rpc-api-openapi.yml
- filename: quant-stakes-api-openapi.yml
  format: yaml
  label: Quant Network Stakes API
  slug: quant-stakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-stakes-api-openapi.yml
- filename: quant-swaps-api-openapi.yml
  format: yaml
  label: Quant Network Swaps API
  slug: quant-swaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-swaps-api-openapi.yml
- filename: quant-tracker-address-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Address API
  slug: quant-tracker-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-address-api-openapi.yml
- filename: quant-tracker-event-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Event API
  slug: quant-tracker-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-event-api-openapi.yml
- filename: quant-tracker-transaction-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Transaction API
  slug: quant-tracker-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-transaction-api-openapi.yml
- filename: quant-user-api-openapi.yml
  format: yaml
  label: Quant Network User API
  slug: quant-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-user-api-openapi.yml
- filename: quant-withdrawals-api-openapi.yml
  format: yaml
  label: Quant Network Withdrawals API
  slug: quant-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-withdrawals-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Quant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quant Network secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quant Network
provider_slug: quant
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'A Keycloak access token (JWT), verified against the realm JWKS

    (signature / issuer / expiry). The caller''s identity is the token''s

    `sub` claim — this is **not** a `clientId`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/quant-overledger-server-openapi.yml
  type: http
- description: 'An Overledger-issued API key of the form `fk_<keyId>.<secret>`, minted via

    `POST /users/me/api-keys`. Accepted on any route and **takes precedence**

    over the `Authorization` header when both are supplied. Resolves to the

    same identity (Keycloak `sub`) as the equivalent Bearer JWT.'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/quant-overledger-server-openapi.yml
  type: apiKey
slug: quant-authentication
source_filename: quant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/quant-overledger-server-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    A Keycloak access token (JWT), verified against the realm JWKS\n    (signature / issuer / expiry). The caller's identity is the token's\n    `sub` claim — this is **not** a `clientId`.\n  sources:\n  - openapi/quant-overledger-server-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    An Overledger-issued API key of the form `fk_<keyId>.<secret>`, minted via\n    `POST /users/me/api-keys`. Accepted on any route and **takes precedence**\n    over the `Authorization` header when both are supplied. Resolves to the\n    same identity (Keycloak `sub`) as the equivalent Bearer JWT.\n  sources:\n  - openapi/quant-overledger-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/authentication/quant-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Blockchain
- Distributed Ledger
- Interoperability
- Overledger
- Smart Contracts
- Digital Assets
- Web3
---
