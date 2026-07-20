---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fidel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fidel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fidel
provider_slug: fidel
scheme_count: 1
schemes:
- example: 'fidel-key: [example key]'
  in: header
  key_kinds:
  - kind: secret-test
    prefix: sk_test_
    usage: server-side calls against the test environment
  - kind: secret-live
    prefix: sk_live_
    usage: server-side calls against the live environment
  - kind: public-test
    prefix: pk_test_
    usage: client-side / SDK card enrollment in the test environment
  - kind: public-live
    prefix: pk_live_
    usage: client-side / SDK card enrollment in the live environment
  name: fidelKey
  parameter_name: fidel-key
  sources:
  - docs
  type: apiKey
slug: fidel-authentication
source_filename: fidel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://reference.fidel.uk/reference/authentication\ndocs: https://reference.fidel.uk/reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  Fidel API authenticates every REST request with a single API key passed in the\n  `fidel-key` HTTP header. Accounts carry both test and live keys, each in a\n  secret (server-side) and public (client/SDK) variant. There is no OAuth 2.0 or\n  OIDC surface, so no scopes artifact applies.\nschemes:\n  - name: fidelKey\n    type: apiKey\n    in: header\n    parameter_name: fidel-key\n    key_kinds:\n      - kind: secret-test\n        prefix: sk_test_\n        usage: server-side calls against the test environment\n      - kind: secret-live\n        prefix: sk_live_\n        usage: server-side calls against the live environment\n      - kind: public-test\n        prefix: pk_test_\n        usage: client-side / SDK card enrollment in the\
  \ test environment\n      - kind: public-live\n        prefix: pk_live_\n        usage: client-side / SDK card enrollment in the live environment\n    example: \"fidel-key: [example key]\"\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fidel/refs/heads/main/authentication/fidel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Card Linking
- Transactions
- Fintech
- Embedded Finance
- Loyalty
- Rewards
- Webhooks
- SDKs
---
