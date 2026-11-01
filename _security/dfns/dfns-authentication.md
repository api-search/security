---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dfns-auth-api-openapi.yml
  format: yaml
  label: Dfns Auth API
  slug: dfns-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-auth-api-openapi.yml
- filename: dfns-keys-api-openapi.yml
  format: yaml
  label: Dfns Keys API
  slug: dfns-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-keys-api-openapi.yml
- filename: dfns-networks-api-openapi.yml
  format: yaml
  label: Dfns Networks API
  slug: dfns-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-networks-api-openapi.yml
- filename: dfns-permissions-api-openapi.yml
  format: yaml
  label: Dfns Permissions API
  slug: dfns-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-permissions-api-openapi.yml
- filename: dfns-policies-api-openapi.yml
  format: yaml
  label: Dfns Policies API
  slug: dfns-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-policies-api-openapi.yml
- filename: dfns-wallets-api-openapi.yml
  format: yaml
  label: Dfns Wallets API
  slug: dfns-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-wallets-api-openapi.yml
- filename: dfns-webhooks-api-openapi.yml
  format: yaml
  label: Dfns Webhooks API
  slug: dfns-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-webhooks-api-openapi.yml
- filename: dfns-address-watches-api-openapi.yml
  format: yaml
  label: Dfns Address Watches API
  slug: dfns-address-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-address-watches-api-openapi.yml
- filename: dfns-agreements-api-openapi.yml
  format: yaml
  label: Dfns Agreements API
  slug: dfns-agreements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-agreements-api-openapi.yml
- filename: dfns-allocations-api-openapi.yml
  format: yaml
  label: Dfns Allocations API
  slug: dfns-allocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-allocations-api-openapi.yml
- filename: dfns-exchanges-api-openapi.yml
  format: yaml
  label: Dfns Exchanges API
  slug: dfns-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-exchanges-api-openapi.yml
- filename: dfns-fee-sponsors-api-openapi.yml
  format: yaml
  label: Dfns Fee Sponsors API
  slug: dfns-fee-sponsors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-fee-sponsors-api-openapi.yml
- filename: dfns-payins-api-openapi.yml
  format: yaml
  label: Dfns Payins API
  slug: dfns-payins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-payins-api-openapi.yml
- filename: dfns-payouts-api-openapi.yml
  format: yaml
  label: Dfns Payouts API
  slug: dfns-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-payouts-api-openapi.yml
- filename: dfns-signers-api-openapi.yml
  format: yaml
  label: Dfns Signers API
  slug: dfns-signers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-signers-api-openapi.yml
- filename: dfns-staking-api-openapi.yml
  format: yaml
  label: Dfns Staking API
  slug: dfns-staking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-staking-api-openapi.yml
- filename: dfns-swaps-api-openapi.yml
  format: yaml
  label: Dfns Swaps API
  slug: dfns-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-swaps-api-openapi.yml
- filename: dfns-tenant-api-openapi.yml
  format: yaml
  label: Dfns Tenant API
  slug: dfns-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-tenant-api-openapi.yml
- filename: dfns-vaults-api-openapi.yml
  format: yaml
  label: Dfns Vaults API
  slug: dfns-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-vaults-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Dfns Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dfns secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dfns
provider_slug: dfns
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'Access token issued to a service account or a logged-in user. Sent as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dfns-openapi.yml
  type: http
- description: The Dfns application (app) id the request is made on behalf of.
  in: header
  name: AppId
  parameter: X-DFNS-APPID
  sources:
  - openapi/dfns-openapi.yml
  type: apiKey
- description: A User Action Signature token proving the caller cryptographically signed the request payload. Required on sensitive mutating operations (transfers, signature generation, key/policy/permission changes).
  in: header
  name: UserAction
  parameter: X-DFNS-USERACTION
  sources:
  - openapi/dfns-openapi.yml
  type: apiKey
slug: dfns-authentication
source_filename: dfns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dfns-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token issued to a service account or a logged-in user. Sent as `Authorization:\n    Bearer <token>`.'\n  sources:\n  - openapi/dfns-openapi.yml\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: X-DFNS-APPID\n  description: The Dfns application (app) id the request is made on behalf of.\n  sources:\n  - openapi/dfns-openapi.yml\n- name: UserAction\n  type: apiKey\n  in: header\n  parameter: X-DFNS-USERACTION\n  description: A User Action Signature token proving the caller cryptographically signed the\n    request payload. Required on sensitive mutating operations (transfers, signature generation,\n    key/policy/permission changes).\n  sources:\n  - openapi/dfns-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dfns/authentication/dfns-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Wallets
- MPC
- Key Management
- Digital Assets
- Web3
- Non-Custodial
---
