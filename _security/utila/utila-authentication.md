---
api_key_in: []
api_specs:
- filename: utila-address-book-api-openapi.yml
  format: yaml
  label: Utila Address Book API
  slug: utila-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-address-book-api-openapi.yml
- filename: utila-assets-api-openapi.yml
  format: yaml
  label: Utila Assets API
  slug: utila-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-assets-api-openapi.yml
- filename: utila-balances-api-openapi.yml
  format: yaml
  label: Utila Balances API
  slug: utila-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-balances-api-openapi.yml
- filename: utila-blockchains-api-openapi.yml
  format: yaml
  label: Utila Blockchains API
  slug: utila-blockchains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-blockchains-api-openapi.yml
- filename: utila-transactions-api-openapi.yml
  format: yaml
  label: Utila Transactions API
  slug: utila-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-transactions-api-openapi.yml
- filename: utila-vaults-api-openapi.yml
  format: yaml
  label: Utila Vaults API
  slug: utila-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-vaults-api-openapi.yml
- filename: utila-wallets-api-openapi.yml
  format: yaml
  label: Utila Wallets API
  slug: utila-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Utila Authentication
name_suffix: Authentication
oauth_flows: []
overview: Utila secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Utila
provider_slug: utila
scheme_count: 1
schemes:
- bearerFormat: JWT
  details:
    claims:
      aud: https://api.utila.io/
      exp: Expiration time, no longer than 1 hour after current time or iat
      sub: Service account email (e.g. my-service-account@vault-aa11bb2cc33dd44.utilaserviceaccount.io)
    header: 'Authorization: Bearer <token>'
    key_type: RSA 4096-bit keypair; public key registered in console
    service_accounts: Created by vault admins in Console under Vault Settings -> Service Accounts; must be added as a member to each vault (admin quorum approval)
    token_generation: Self-signed JWT using the service account RSA private key, algorithm RS256
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/utila-v2-openapi-original.json
  type: http
slug: utila-authentication
source_filename: utila-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.utila.io/reference/authentication\ndocs: https://docs.utila.io/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  notes: Service-account JWT bearer authentication. Clients self-sign short-lived\n    JWTs (RS256) with the service account's 4096-bit RSA private key; the public\n    key is registered in the Utila Console (Vault Settings -> Service Accounts,\n    subject to admin quorum approval).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/utila-v2-openapi-original.json\n  details:\n    token_generation: Self-signed JWT using the service account RSA private key,\n      algorithm RS256\n    claims:\n      sub: Service account email (e.g. my-service-account@vault-aa11bb2cc33dd44.utilaserviceaccount.io)\n      aud: https://api.utila.io/\n      exp: Expiration time, no longer than 1 hour after\
  \ current time or iat\n    header: 'Authorization: Bearer <token>'\n    key_type: RSA 4096-bit keypair; public key registered in console\n    service_accounts: Created by vault admins in Console under Vault Settings ->\n      Service Accounts; must be added as a member to each vault (admin quorum\n      approval)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/authentication/utila-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web3
- Digital Assets
- Stablecoins
- Custody
- MPC Wallets
- Blockchain
- Payments
- Treasury
---
