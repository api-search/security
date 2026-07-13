---
api_key_in:
- header
api_specs:
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Wallets API
  slug: dfns-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Keys API
  slug: dfns-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Transfers API
  slug: dfns-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Transactions API
  slug: dfns-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Signatures API
  slug: dfns-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Policy Engine and Approvals API
  slug: dfns-policy-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Webhooks API
  slug: dfns-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Permissions and Auth API
  slug: dfns-permissions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Service Accounts API
  slug: dfns-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
- filename: dfns-openapi.yml
  format: yaml
  label: Dfns Networks API
  slug: dfns-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/authentication/dfns-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Wallets
- MPC
- Key Management
- Digital Assets
- Web3
- Non-Custodial
---
