---
api_key_in: []
auth_types:
- apiKey
- http
description: 'How clients authenticate to Defined''s Codex GraphQL API (https://graph.codex.io/graphql). Three mechanisms: long-lived secret API keys, short-lived JWTs minted server-side for untrusted clients, and keyless pay-per-request access for agents via the Machine Payments Protocol.'
kind: authentication
layout: security
method: searched
name: Defined Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defined secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Defined
provider_slug: defined
scheme_count: 3
schemes:
- bearer_prefix: false
  description: Long-lived secret API key obtained from the Codex dashboard, passed in the Authorization header with NO Bearer prefix. Used for server-side requests.
  docs: https://docs.codex.io/get-started.md
  format: 'Authorization: <API_KEY>'
  header: Authorization
  in: header
  name: secretApiKey
  type: apiKey
- bearer_prefix: true
  description: Short-lived JWT minted by the createApiTokens mutation for untrusted contexts (browsers, user-facing apps). Supports configurable requestLimit and expiresIn windows. Cannot be used for API-token management operations. Invalid/expired tokens return HTTP 401.
  docs: https://docs.codex.io/concepts/authentication.md
  format: 'Authorization: Bearer <token>'
  name: shortLivedJwt
  scheme: bearer
  type: http
- description: Keyless, pay-per-request access for AI agents over HTTP 402 via the Machine Payments Protocol (MPP) — no API key required.
  docs: https://docs.codex.io/agents/mpp.md
  name: machinePaymentsProtocol
  scheme: http-402
  type: http
slug: defined-authentication
source_filename: defined-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docs.codex.io/concepts/authentication.md and\n  https://docs.codex.io/llms.txt — Codex is a GraphQL API (no OpenAPI\n  securitySchemes), so this profile is captured from the published auth docs.\ndescription: >-\n  How clients authenticate to Defined's Codex GraphQL API\n  (https://graph.codex.io/graphql). Three mechanisms: long-lived secret API keys,\n  short-lived JWTs minted server-side for untrusted clients, and keyless\n  pay-per-request access for agents via the Machine Payments Protocol.\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: secretApiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  format: \"Authorization: <API_KEY>\"\n  bearer_prefix: false\n  description: >-\n    Long-lived secret API key obtained from the Codex dashboard, passed in the\n    Authorization header with NO Bearer prefix. Used for server-side requests.\n  docs: https://docs.codex.io/get-started.md\n- name:\
  \ shortLivedJwt\n  type: http\n  scheme: bearer\n  format: \"Authorization: Bearer <token>\"\n  bearer_prefix: true\n  description: >-\n    Short-lived JWT minted by the createApiTokens mutation for untrusted contexts\n    (browsers, user-facing apps). Supports configurable requestLimit and\n    expiresIn windows. Cannot be used for API-token management operations.\n    Invalid/expired tokens return HTTP 401.\n  docs: https://docs.codex.io/concepts/authentication.md\n- name: machinePaymentsProtocol\n  type: http\n  scheme: http-402\n  description: >-\n    Keyless, pay-per-request access for AI agents over HTTP 402 via the Machine\n    Payments Protocol (MPP) — no API key required.\n  docs: https://docs.codex.io/agents/mpp.md\nnotes: >-\n  There is no OAuth 2.0 / OIDC authorization-code flow and no per-scope\n  permission model documented; access is gated by API key + plan (see\n  lifecycle/defined-lifecycle.yml and Pricing).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defined/refs/heads/main/authentication/defined-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Cryptocurrency
- Blockchain
- DeFi
- Market Data
- Trading
- GraphQL
- Web3
- Prediction Markets
- API
---
