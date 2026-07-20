---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fidel Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: FIDEL API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FIDEL API
provider_slug: fidel-api
scheme_count: 1
schemes:
- description: 'All Fidel API requests authenticate with a secret API key passed in the Fidel-Key HTTP header. Keys are environment-scoped: Test keys access the test environment and Live keys access the live environment. There are two key classes - API keys (server-side, direct REST API access) and SDK keys (used to link the Web/iOS/Android/React Native SDKs to your account). Keys are created, viewed, and revoked in the Fidel Dashboard under Account Settings > Plan.'
  in: header
  name: FidelKey
  parameter_name: Fidel-Key
  sources:
  - docs.fidelapi.com
  type: apiKey
slug: fidel-api-authentication
source_filename: fidel-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fidelapi.com/docs/select (Getting Started - Managing API Keys)\ndocs: https://reference.fidel.uk/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: FidelKey\n    type: apiKey\n    in: header\n    parameter_name: Fidel-Key\n    description: >-\n      All Fidel API requests authenticate with a secret API key passed in the\n      Fidel-Key HTTP header. Keys are environment-scoped: Test keys access the\n      test environment and Live keys access the live environment. There are two\n      key classes - API keys (server-side, direct REST API access) and SDK keys\n      (used to link the Web/iOS/Android/React Native SDKs to your account).\n      Keys are created, viewed, and revoked in the Fidel Dashboard under\n      Account Settings > Plan.\n    sources: [docs.fidelapi.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fidel-api/refs/heads/main/authentication/fidel-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Card Linking
- Payments
- Transactions
- Webhooks
- SDK
- Card-Linked Offers
- Financial Data
---
