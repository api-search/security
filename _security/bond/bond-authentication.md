---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bond Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bond secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bond
provider_slug: bond
scheme_count: 2
schemes:
- description: The Identity portion of the Bond API key (e.g. a UUID). Sent on every request alongside the Authorization header.
  in: header
  name: Identity
  parameter: Identity
  sources:
  - https://docs.bond.tech/reference/authentication
  type: apiKey
- description: The secret Authorization portion of the Bond API key. Sent on every request alongside the Identity header.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - https://docs.bond.tech/reference/authentication
  type: apiKey
slug: bond-authentication
source_filename: bond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bond.tech/reference/authentication\ndocs: https://docs.bond.tech/reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Bond uses a two-part API key: an Identity value and an Authorization value,\n    both sent as request headers. The key identifies the Bond account (brand),\n    not an individual team member. Keys are created and managed in the Bond Portal.\nschemes:\n  - name: Identity\n    type: apiKey\n    in: header\n    parameter: Identity\n    description: >-\n      The Identity portion of the Bond API key (e.g. a UUID). Sent on every\n      request alongside the Authorization header.\n    sources: [https://docs.bond.tech/reference/authentication]\n  - name: Authorization\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      The secret Authorization portion of the Bond API key. Sent on every request\n      alongside\
  \ the Identity header.\n    sources: [https://docs.bond.tech/reference/authentication]\nrequired_headers:\n  - name: Identity\n    required: true\n  - name: Authorization\n    required: true\n  - name: content-type\n    required: true\n    values: application/json\n    applies_to: [POST, PATCH, DELETE]\nkey_management:\n  portal: https://portal.bond.tech\n  notes: >-\n    An account may hold any number of API keys. All keys currently grant access\n    to every endpoint on the platform. Separate keys exist per environment\n    (sandbox vs production).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/authentication/bond-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Card Issuing
- Deposit Accounts
- Money Movement
- ACH
- KYC
- KYB
- Credit
---
