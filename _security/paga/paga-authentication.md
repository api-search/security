---
api_key_in: []
api_specs:
- filename: paga-openapi.yml
  format: yaml
  label: Paga Collect API
  slug: paga-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Business API
  slug: paga-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Direct Debit API
  slug: paga-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: modeled-from-docs
name: Paga Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paga secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paga
provider_slug: paga
scheme_count: 4
schemes:
- appliesTo:
  - Paga Collect API
  - Paga Direct Debit API
  description: Collect API and Direct Debit API authenticate with HTTP Basic using base64(publicKey:secretKey) - the account principal (public key) and credential (secret key).
  name: basic_auth
  scheme: basic
  sources:
  - https://developer-docs.paga.com/docs/paga-collect-api
  type: http
- appliesTo:
  - Paga Business API
  description: Business API public key (principal / merchant public ID), sent as a header.
  headerName: principal
  in: header
  name: principal
  sources:
  - https://developer-docs.paga.com/docs/introduction
  type: apiKey
- appliesTo:
  - Paga Business API
  description: Business API secret key (credential / password), sent as a header.
  headerName: credentials
  in: header
  name: credentials
  sources:
  - https://developer-docs.paga.com/docs/introduction
  type: apiKey
- appliesTo:
  - Paga Business API
  - Paga Collect API
  - Paga Direct Debit API
  description: 'Every operation additionally requires a SHA-512 hash header computed over an operation-specific ordered concatenation of request parameters followed by the account hash key (HMAC key from the Business dashboard), joined with no separators. Example order for Deposit To Bank: referenceNumber + amount + destinationBankUUID + destinationBankAccountNumber + hashKey. The hash key itself is never transmitted.'
  headerName: hash
  in: header
  name: hash
  sources:
  - https://developer-docs.paga.com/docs/handling-hash
  type: apiKey
slug: paga-authentication
source_filename: paga-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: modeled-from-docs\nsource: https://developer-docs.paga.com/docs/introduction\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: >-\n    Collect API and Direct Debit API authenticate with HTTP Basic using\n    base64(publicKey:secretKey) - the account principal (public key) and\n    credential (secret key).\n  appliesTo:\n  - Paga Collect API\n  - Paga Direct Debit API\n  sources:\n  - https://developer-docs.paga.com/docs/paga-collect-api\n- name: principal\n  type: apiKey\n  in: header\n  headerName: principal\n  description: Business API public key (principal / merchant public ID), sent as a header.\n  appliesTo:\n  - Paga Business API\n  sources:\n  - https://developer-docs.paga.com/docs/introduction\n- name: credentials\n  type: apiKey\n  in: header\n  headerName: credentials\n  description: Business API secret key (credential / password), sent as a header.\n  appliesTo:\n\
  \  - Paga Business API\n  sources:\n  - https://developer-docs.paga.com/docs/introduction\n- name: hash\n  type: apiKey\n  in: header\n  headerName: hash\n  description: >-\n    Every operation additionally requires a SHA-512 hash header computed over an\n    operation-specific ordered concatenation of request parameters followed by\n    the account hash key (HMAC key from the Business dashboard), joined with no\n    separators. Example order for Deposit To Bank: referenceNumber + amount +\n    destinationBankUUID + destinationBankAccountNumber + hashKey. The hash key\n    itself is never transmitted.\n  appliesTo:\n  - Paga Business API\n  - Paga Collect API\n  - Paga Direct Debit API\n  sources:\n  - https://developer-docs.paga.com/docs/handling-hash\nnotes: >-\n  Credentials (public key, secret key, hash key) are issued from the Paga\n  Business Account dashboard under Developer Tools > API keys, with separate\n  test and live sets. The Business API additionally requires the caller's\
  \ IP\n  address to be whitelisted before access is granted. Paga Connect is a\n  separate OAuth 2.0 hosted-checkout flow and is not covered by the hash scheme\n  above.\nregions:\n- Nigeria\ncurrency: NGN\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/authentication/paga-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Payments
- Mobile Money
- Fintech
- Collections
- Nigeria
---
