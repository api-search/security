---
api_key_in: []
api_specs:
- filename: syndicate-api-key-manager-admin-api-openapi.yml
  format: yaml
  label: Syndicate api-key-manager > admin API
  slug: syndicate-api-key-manager-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/openapi/syndicate-api-key-manager-admin-api-openapi.yml
- filename: syndicate-call-api-openapi.yml
  format: yaml
  label: Syndicate call API
  slug: syndicate-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/openapi/syndicate-call-api-openapi.yml
- filename: syndicate-transact-api-openapi.yml
  format: yaml
  label: Syndicate transact API
  slug: syndicate-transact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/openapi/syndicate-transact-api-openapi.yml
- filename: syndicate-wallet-api-openapi.yml
  format: yaml
  label: Syndicate wallet API
  slug: syndicate-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/openapi/syndicate-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Syndicate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syndicate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Syndicate
provider_slug: syndicate
scheme_count: 1
schemes:
- name: default
  scheme: bearer
  sources:
  - openapi/syndicate-transaction-cloud-openapi-original.yml
  type: http
slug: syndicate-authentication
source_filename: syndicate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/syndicate-transaction-cloud-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: default\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/syndicate-transaction-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/authentication/syndicate-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Web3
- Ethereum
- Transactions
- Wallets
- EVM
- Infrastructure
- Signing
- Webhooks
- Cryptography
---
