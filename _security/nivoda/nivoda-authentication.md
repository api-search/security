---
api_key_in: []
auth_types:
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Nivoda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nivoda secures its APIs with bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nivoda
provider_slug: nivoda
scheme_count: 2
schemes:
- endpoint: https://integrations.nivoda.net/api/diamonds
  header: Authorization
  in: header
  name: BearerToken
  obtained_via: authenticate.username_and_password(username, password) { token }
  scheme: bearer
  sources:
  - examples/orders/nodejs-orders.js
  - examples/holds/nodejs-holds.js
  - examples/search/graphql-search.gql
  type: http
- applies_to: https://integrations.nivoda.net/api/diamonds-graphiql
  in: header
  name: GraphiQLBasicAuth
  note: Public browse-only credentials for the GraphiQL explorer UI.
  scheme: basic
  sources:
  - README.md
  type: http
slug: nivoda-authentication
source_filename: nivoda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://bitbucket.org/nivoda/nivoda-api/src/main/\ndocs: https://bitbucket.org/nivoda/nivoda-api/src/main/\nsummary:\n  types: [bearer]\n  token_acquisition: graphql-login-mutation\n  credentials: nivoda-platform-username-password\n  token_header: Authorization Bearer\nnotes: >-\n  The Nivoda GraphQL API is not OpenAPI/OAuth-based. A client first runs the\n  `authenticate` query with `username_and_password(username, password)` (the same\n  credentials used to log in to the Nivoda platform) which returns a session\n  `token`. That token is then sent as an `Authorization: Bearer <token>` header\n  on all subsequent query/mutation requests. In the GraphiQL explorer the token\n  is supplied by wrapping the operation in `as(token: $token) { ... }`. The\n  GraphiQL explorer page itself is additionally gated by HTTP Basic auth\n  (nivoda-api-docs / nivoda-graphiql) documented publicly for browsing. Staging\n  credentials are shared\
  \ on request; production login is activated by a Nivoda\n  account manager after signing the Nivoda Feed Agreement.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  obtained_via: 'authenticate.username_and_password(username, password) { token }'\n  endpoint: https://integrations.nivoda.net/api/diamonds\n  sources: [examples/orders/nodejs-orders.js, examples/holds/nodejs-holds.js, examples/search/graphql-search.gql]\n- name: GraphiQLBasicAuth\n  type: http\n  scheme: basic\n  in: header\n  applies_to: https://integrations.nivoda.net/api/diamonds-graphiql\n  note: Public browse-only credentials for the GraphiQL explorer UI.\n  sources: [README.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nivoda/refs/heads/main/authentication/nivoda-authentication.yml
summary_line: bearer · 2 schemes
tags:
- Company
- Diamonds
- Gemstones
- Jewelry
- Marketplace
- B2B
- GraphQL
- Inventory
- E-commerce
---
