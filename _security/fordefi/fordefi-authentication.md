---
api_key_in: []
api_specs:
- filename: fordefi-address-book-api-openapi.yml
  format: yaml
  label: Fordefi Address Book API
  slug: fordefi-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-address-book-api-openapi.yml
- filename: fordefi-assets-api-openapi.yml
  format: yaml
  label: Fordefi Assets API
  slug: fordefi-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-assets-api-openapi.yml
- filename: fordefi-audit-log-api-openapi.yml
  format: yaml
  label: Fordefi Audit Log API
  slug: fordefi-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-audit-log-api-openapi.yml
- filename: fordefi-authorization-tokens-api-openapi.yml
  format: yaml
  label: Fordefi Authorization Tokens API
  slug: fordefi-authorization-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-authorization-tokens-api-openapi.yml
- filename: fordefi-batch-transactions-api-openapi.yml
  format: yaml
  label: Fordefi Batch Transactions API
  slug: fordefi-batch-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-batch-transactions-api-openapi.yml
- filename: fordefi-blockchains-api-openapi.yml
  format: yaml
  label: Fordefi Blockchains API
  slug: fordefi-blockchains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-blockchains-api-openapi.yml
- filename: fordefi-enclave-keys-api-openapi.yml
  format: yaml
  label: Fordefi Enclave Keys API
  slug: fordefi-enclave-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-enclave-keys-api-openapi.yml
- filename: fordefi-end-users-api-openapi.yml
  format: yaml
  label: Fordefi End Users API
  slug: fordefi-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-end-users-api-openapi.yml
- filename: fordefi-exports-api-openapi.yml
  format: yaml
  label: Fordefi Exports API
  slug: fordefi-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-exports-api-openapi.yml
- filename: fordefi-organizations-api-openapi.yml
  format: yaml
  label: Fordefi Organizations API
  slug: fordefi-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-organizations-api-openapi.yml
- filename: fordefi-swaps-api-openapi.yml
  format: yaml
  label: Fordefi Swaps API
  slug: fordefi-swaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-swaps-api-openapi.yml
- filename: fordefi-transactions-api-openapi.yml
  format: yaml
  label: Fordefi Transactions API
  slug: fordefi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-transactions-api-openapi.yml
- filename: fordefi-user-groups-api-openapi.yml
  format: yaml
  label: Fordefi User Groups API
  slug: fordefi-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-user-groups-api-openapi.yml
- filename: fordefi-users-api-openapi.yml
  format: yaml
  label: Fordefi Users API
  slug: fordefi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-users-api-openapi.yml
- filename: fordefi-vault-groups-api-openapi.yml
  format: yaml
  label: Fordefi Vault Groups API
  slug: fordefi-vault-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-vault-groups-api-openapi.yml
- filename: fordefi-vaults-api-openapi.yml
  format: yaml
  label: Fordefi Vaults API
  slug: fordefi-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-vaults-api-openapi.yml
- filename: fordefi-webhooks-api-openapi.yml
  format: yaml
  label: Fordefi Webhooks API
  slug: fordefi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fordefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fordefi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fordefi
provider_slug: fordefi
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: 'Authorization: Bearer {api_access_token}'
  name: bearerAuth
  note: API access token (JWT) issued for an API User. Sensitive/state-changing requests additionally require an ECDSA (NIST P-256) signature over "${path}|${timestamp}|${body}" sent in x-signature with x-timestamp, produced by the API Signer whose public key is registered with the API User.
  scheme: bearer
  sources:
  - openapi/fordefi-openapi-original.json
  type: http
slug: fordefi-authentication
source_filename: fordefi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fordefi-openapi-original.json\ndocs: https://docs.fordefi.com/developers/authentication\nsummary:\n  types:\n  - http\n  request_signing: ECDSA over NIST P-256 (x-signature/x-timestamp) for state-changing ops\n  transport: HTTPS only\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer {api_access_token}'\n  note: >-\n    API access token (JWT) issued for an API User. Sensitive/state-changing\n    requests additionally require an ECDSA (NIST P-256) signature over\n    \"${path}|${timestamp}|${body}\" sent in x-signature with x-timestamp, produced\n    by the API Signer whose public key is registered with the API User.\n  sources:\n  - openapi/fordefi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/authentication/fordefi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cryptocurrency
- Digital Assets
- Wallets
- Custody
- Blockchain
- DeFi
- MPC
- Payments
---
