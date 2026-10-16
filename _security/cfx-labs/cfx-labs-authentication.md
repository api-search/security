---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cfx-labs-cash-api-openapi.yml
  format: yaml
  label: CFX Labs Cash API
  slug: cfx-labs-cash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-cash-api-openapi.yml
- filename: cfx-labs-deposit-api-openapi.yml
  format: yaml
  label: CFX Labs Deposit API
  slug: cfx-labs-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-deposit-api-openapi.yml
- filename: cfx-labs-deposit-memos-api-openapi.yml
  format: yaml
  label: CFX Labs Deposit Memos API
  slug: cfx-labs-deposit-memos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-deposit-memos-api-openapi.yml
- filename: cfx-labs-escrow-transfers-api-openapi.yml
  format: yaml
  label: CFX Labs Escrow Transfers API
  slug: cfx-labs-escrow-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-escrow-transfers-api-openapi.yml
- filename: cfx-labs-identity-api-openapi.yml
  format: yaml
  label: CFX Labs Identity API
  slug: cfx-labs-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-identity-api-openapi.yml
- filename: cfx-labs-identity-documents-api-openapi.yml
  format: yaml
  label: CFX Labs Identity Documents API
  slug: cfx-labs-identity-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-identity-documents-api-openapi.yml
- filename: cfx-labs-ledger-accounts-api-openapi.yml
  format: yaml
  label: CFX Labs Ledger Accounts API
  slug: cfx-labs-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-ledger-accounts-api-openapi.yml
- filename: cfx-labs-payment-instruments-api-openapi.yml
  format: yaml
  label: CFX Labs Payment Instruments API
  slug: cfx-labs-payment-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-payment-instruments-api-openapi.yml
- filename: cfx-labs-products-api-openapi.yml
  format: yaml
  label: CFX Labs Products API
  slug: cfx-labs-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-products-api-openapi.yml
- filename: cfx-labs-transfer-requests-api-openapi.yml
  format: yaml
  label: CFX Labs Transfer Requests API
  slug: cfx-labs-transfer-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-transfer-requests-api-openapi.yml
- filename: cfx-labs-us-bank-ach-api-openapi.yml
  format: yaml
  label: CFX Labs US Bank ACH API
  slug: cfx-labs-us-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-us-bank-ach-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Cfx Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: CFX Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CFX Labs
provider_slug: cfx-labs
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/cash-deposit-simulator-api.json
  - openapi/deposit-api.json
  - openapi/escrow-transfer-api.json
  - openapi/events-api.json
  - openapi/identity-api.json
  type: apiKey
- in: header
  name: ApiSecretAuth
  parameter: x-api-secret
  sources:
  - openapi/cash-deposit-simulator-api.json
  - openapi/deposit-api.json
  - openapi/escrow-transfer-api.json
  - openapi/events-api.json
  - openapi/identity-api.json
  type: apiKey
slug: cfx-labs-authentication
source_filename: cfx-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/cash-deposit-simulator-api.json, openapi/deposit-api.json, openapi/escrow-transfer-api.json,\n  openapi/events-api.json, openapi/identity-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/cash-deposit-simulator-api.json\n  - openapi/deposit-api.json\n  - openapi/escrow-transfer-api.json\n  - openapi/events-api.json\n  - openapi/identity-api.json\n- name: ApiSecretAuth\n  type: apiKey\n  in: header\n  parameter: x-api-secret\n  sources:\n  - openapi/cash-deposit-simulator-api.json\n  - openapi/deposit-api.json\n  - openapi/escrow-transfer-api.json\n  - openapi/events-api.json\n  - openapi/identity-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/authentication/cfx-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- fintech
- banking
- payments
- API
- programmable
- company
---
