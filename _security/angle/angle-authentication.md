---
api_key_in: []
api_specs:
- filename: angle-api-openapi.json
  format: json
  label: Angle API
  slug: angle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/angle/refs/heads/main/openapi/angle-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Angle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Angle declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Angle
provider_slug: angle
scheme_count: 1
schemes:
- name: BasicAuth
  note: The older OpenAPI published in the AngleProtocol/swagger GitHub repository declares a `BasicAuth` securityScheme under components.securitySchemes, but it is never applied — there is no root-level `security` object and no operation-level `security` on any of its 13 paths. The newer specification served live from https://api.angle.money/api-docs/ drops the scheme entirely.
  scheme: basic
  sources:
  - openapi/angle-api-openapi-github.yaml
  status: declared-not-applied
  type: http
slug: angle-authentication
source_filename: angle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/angle-api-openapi.json + openapi/angle-api-openapi-github.yaml + live probe of https://api.angle.money\nsummary:\n  model: none\n  authenticated: false\n  description: >-\n    The Angle API is a public, read-only data API. No credential is required. Every\n    published operation is an HTTP GET over a public host, and the API returned data\n    on an unauthenticated request during this pass.\n  types: []\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  status: declared-not-applied\n  sources:\n  - openapi/angle-api-openapi-github.yaml\n  note: >-\n    The older OpenAPI published in the AngleProtocol/swagger GitHub repository declares\n    a `BasicAuth` securityScheme under components.securitySchemes, but it is never\n    applied — there is no root-level `security` object and no operation-level `security`\n    on any of its 13 paths. The newer specification served live from\n    https://api.angle.money/api-docs/\
  \ drops the scheme entirely.\nevidence:\n- check: unauthenticated request succeeds\n  request: GET https://api.angle.money/v1/activeChains\n  status: 200\n  result: '{\"borrowModule\":[\"1\",\"10\",\"137\",\"42161\",\"43114\"]}'\n  date: '2026-07-19'\n- check: live spec declares no securitySchemes\n  source: https://api.angle.money/api-docs/\n  result: components.securitySchemes absent; no root security object\nnotes:\n- No API keys, no OAuth 2.0, no OpenID Connect and no mutual TLS are published for\n  this API, so scopes/ is intentionally not produced.\n- Authorization in the Angle system is on-chain rather than at the API layer — state\n  changes are performed by signing transactions with a wallet against the protocol's\n  smart contracts. Several endpoints (`/v1/leverage`, `/v1/deleverage`,\n  `/v1/integrators/payload/deposit`, `/v1/integrators/payload/withdraw`) only BUILD\n  unsigned transaction payloads; the caller signs and submits them on chain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angle/refs/heads/main/authentication/angle-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Stablecoins
- Decentralized Finance
- Blockchain
- Cryptocurrency
- Smart Contracts
- Ethereum
- SDK
---
