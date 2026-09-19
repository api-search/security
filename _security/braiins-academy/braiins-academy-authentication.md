---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: braiins-academy-accounts-api-openapi.yml
  format: yaml
  label: Braiins Accounts API
  slug: braiins-academy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-accounts-api-openapi.yml
- filename: braiins-academy-actions-api-openapi.yml
  format: yaml
  label: Braiins Actions API
  slug: braiins-academy-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-actions-api-openapi.yml
- filename: braiins-academy-advanced-settings-api-openapi.yml
  format: yaml
  label: Braiins Advanced Settings API
  slug: braiins-academy-advanced-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-advanced-settings-api-openapi.yml
- filename: braiins-academy-authentication-api-openapi.yml
  format: yaml
  label: Braiins Authentication API
  slug: braiins-academy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-authentication-api-openapi.yml
- filename: braiins-academy-bid-orders-api-openapi.yml
  format: yaml
  label: Braiins Bid orders API
  slug: braiins-academy-bid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-bid-orders-api-openapi.yml
- filename: braiins-academy-configuration-api-openapi.yml
  format: yaml
  label: Braiins Configuration API
  slug: braiins-academy-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-configuration-api-openapi.yml
- filename: braiins-academy-contracts-api-openapi.yml
  format: yaml
  label: Braiins Contracts API
  slug: braiins-academy-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-contracts-api-openapi.yml
- filename: braiins-academy-cooling-api-openapi.yml
  format: yaml
  label: Braiins Cooling API
  slug: braiins-academy-cooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-cooling-api-openapi.yml
- filename: braiins-academy-documentation-api-openapi.yml
  format: yaml
  label: Braiins Documentation API
  slug: braiins-academy-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-documentation-api-openapi.yml
- filename: braiins-academy-license-api-openapi.yml
  format: yaml
  label: Braiins License API
  slug: braiins-academy-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-license-api-openapi.yml
- filename: braiins-academy-market-configuration-api-openapi.yml
  format: yaml
  label: Braiins Market configuration API
  slug: braiins-academy-market-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-market-configuration-api-openapi.yml
- filename: braiins-academy-market-data-api-openapi.yml
  format: yaml
  label: Braiins Market data API
  slug: braiins-academy-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-market-data-api-openapi.yml
- filename: braiins-academy-miner-api-openapi.yml
  format: yaml
  label: Braiins Miner API
  slug: braiins-academy-miner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-miner-api-openapi.yml
- filename: braiins-academy-network-api-openapi.yml
  format: yaml
  label: Braiins Network API
  slug: braiins-academy-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-network-api-openapi.yml
- filename: braiins-academy-performance-api-openapi.yml
  format: yaml
  label: Braiins Performance API
  slug: braiins-academy-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-performance-api-openapi.yml
- filename: braiins-academy-pools-api-openapi.yml
  format: yaml
  label: Braiins Pools API
  slug: braiins-academy-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-pools-api-openapi.yml
- filename: braiins-academy-upgrade-api-openapi.yml
  format: yaml
  label: Braiins Upgrade API
  slug: braiins-academy-upgrade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-upgrade-api-openapi.yml
- filename: braiins-academy-version-api-openapi.yml
  format: yaml
  label: Braiins Version API
  slug: braiins-academy-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/openapi/braiins-academy-version-api-openapi.yml
auth_types:
- apiKey
- http
description: 'Braiins runs three independent authentication models, one per API surface. There is no single Braiins identity across them: a Braiins Pool access-profile token does not authenticate Braiins Hashpower, and neither reaches a miner running Braiins OS, whose Public API authenticates against the device itself.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Braiins Academy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Braiins secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Braiins
provider_slug: braiins-academy
scheme_count: 3
schemes:
- acl_roles:
  - owner
  - read-only
  - contract-cancel-fee-public
  anonymous_endpoints: /spot/orderbook, /spot/trades, /spot/bars, /spot/stats are callable with no credential; /contract/cancel-fee accepts an optional key and returns generic fee layers without one.
  api: braiins-academy:braiins-hashpower-api
  description: API credential issued for a Braiins Hashpower account. The credential's ACL role and resource ownership determine which authenticated operations and records are available.
  docs: https://academy.braiins.com/braiins-hashpower/api.md
  in: header
  issuance: Tokens are displayed once, immediately after Hashpower account registration at https://hashpower.braiins.com. Braiins states they are shown only once.
  name: ApiKey
  parameter: apikey
  sources:
  - openapi/braiins-academy-braiins-hashpower-openapi.yml
  token_types:
  - access: Full access to all endpoints including trading
    name: Owner Token
  - access: Market data and account viewing only
    name: Read-only Token
  type: apiKey
- alternate_parameter: X-Pool-Auth-Token
  api: braiins-academy:braiins-pool-api
  description: Braiins Pool access-profile token. Each access profile carries its own token; a profile must have "Allow access to web APIs" enabled before a token can be generated.
  docs: https://academy.braiins.com/braiins-pool/monitoring.md
  in: header
  issuance: Settings > Access Profiles > Allow access to web APIs > Generate New token
  name: PoolAuthToken
  parameter: Pool-Auth-Token
  revocation: Regenerating a profile's token immediately invalidates the previous one. Tokens are scoped to the permissions of their access profile.
  sources:
  - https://academy.braiins.com/braiins-pool/monitoring.md
  type: apiKey
- api: braiins-academy:braiins-os-api
  description: Braiins OS Public API device session token. POST /api/v1/auth/login with the miner's username and password returns a token that must be sent in the Authorization header of subsequent requests. Authentication is against the individual miner, not a Braiins account.
  docs: https://academy.braiins.com/braiins-os/papi-about.md
  grpc_equivalent: braiins.bos.v1.AuthenticationService (grpc/braiins-academy-bos-authentication.proto) — the gRPC surface issues the same session token.
  in: header
  login_operation: login
  name: BosSessionToken
  note: The published OpenAPI declares no components.securitySchemes and no top-level security[], so the Authorization requirement is documented in the login operation description and in the BOS gRPC docs rather than expressed in the machine-readable contract. Recorded as a contract gap, not as an absent auth model.
  parameter: Authorization
  password_operation: setPassword
  scheme: bearer
  sources:
  - openapi/braiins-academy-braiins-os-public-rest-api-openapi.json
  - grpc/braiins-academy-bos-authentication.proto
  type: http
slug: braiins-academy-authentication
source_filename: braiins-academy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://academy.braiins.com/braiins-hashpower/api.md,\n  https://academy.braiins.com/braiins-pool/monitoring.md,\n  https://developer.braiins-os.com/latest/openapi.json,\n  https://github.com/braiins/bos-plus-api (proto/bos/v1/authentication.proto);\n  the Hashpower securityScheme was derived from\n  openapi/braiins-academy-braiins-hashpower-openapi.yml and upgraded from the docs.\ndescription: >-\n  Braiins runs three independent authentication models, one per API surface. There is no\n  single Braiins identity across them: a Braiins Pool access-profile token does not\n  authenticate Braiins Hashpower, and neither reaches a miner running Braiins OS, whose\n  Public API authenticates against the device itself.\nsummary:\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: ApiKey\n    api: braiins-academy:braiins-hashpower-api\n\
  \    type: apiKey\n    in: header\n    parameter: apikey\n    description: >-\n      API credential issued for a Braiins Hashpower account. The credential's ACL role and\n      resource ownership determine which authenticated operations and records are available.\n    token_types:\n      - name: Owner Token\n        access: Full access to all endpoints including trading\n      - name: Read-only Token\n        access: Market data and account viewing only\n    issuance: >-\n      Tokens are displayed once, immediately after Hashpower account registration at\n      https://hashpower.braiins.com. Braiins states they are shown only once.\n    acl_roles:\n      - owner\n      - read-only\n      - contract-cancel-fee-public\n    anonymous_endpoints: >-\n      /spot/orderbook, /spot/trades, /spot/bars, /spot/stats are callable with no credential;\n      /contract/cancel-fee accepts an optional key and returns generic fee layers without one.\n    docs: https://academy.braiins.com/braiins-hashpower/api.md\n\
  \    sources:\n      - openapi/braiins-academy-braiins-hashpower-openapi.yml\n  - name: PoolAuthToken\n    api: braiins-academy:braiins-pool-api\n    type: apiKey\n    in: header\n    parameter: Pool-Auth-Token\n    alternate_parameter: X-Pool-Auth-Token\n    description: >-\n      Braiins Pool access-profile token. Each access profile carries its own token; a profile\n      must have \"Allow access to web APIs\" enabled before a token can be generated.\n    issuance: Settings > Access Profiles > Allow access to web APIs > Generate New token\n    revocation: >-\n      Regenerating a profile's token immediately invalidates the previous one. Tokens are\n      scoped to the permissions of their access profile.\n    docs: https://academy.braiins.com/braiins-pool/monitoring.md\n    sources:\n      - https://academy.braiins.com/braiins-pool/monitoring.md\n  - name: BosSessionToken\n    api: braiins-academy:braiins-os-api\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n\
  \    description: >-\n      Braiins OS Public API device session token. POST /api/v1/auth/login with the miner's\n      username and password returns a token that must be sent in the Authorization header of\n      subsequent requests. Authentication is against the individual miner, not a Braiins account.\n    login_operation: login\n    password_operation: setPassword\n    grpc_equivalent: >-\n      braiins.bos.v1.AuthenticationService (grpc/braiins-academy-bos-authentication.proto) —\n      the gRPC surface issues the same session token.\n    note: >-\n      The published OpenAPI declares no components.securitySchemes and no top-level security[],\n      so the Authorization requirement is documented in the login operation description and in\n      the BOS gRPC docs rather than expressed in the machine-readable contract. Recorded as a\n      contract gap, not as an absent auth model.\n    docs: https://academy.braiins.com/braiins-os/papi-about.md\n    sources:\n      - openapi/braiins-academy-braiins-os-public-rest-api-openapi.json\n\
  \      - grpc/braiins-academy-bos-authentication.proto\ngaps:\n  - >-\n    Braiins OS Public REST API publishes no securitySchemes in its OpenAPI even though\n    /api/v1/auth/login issues a bearer token — an agent reading only the spec cannot tell\n    which operations require the token.\n  - >-\n    No OAuth 2.0 or OpenID Connect surface exists on any Braiins API; there is no delegated\n    (third-party) authorization path, so scopes/ is not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/authentication/braiins-academy-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Bitcoin Mining
- Cryptocurrency
- Mining Pool
- Mining Firmware
- Blockchain
- Stratum V2
- Hashrate Marketplace
- Mining Management
- ASIC
- Energy
---
