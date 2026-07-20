---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hypercore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypercore secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hypercore
provider_slug: hypercore
scheme_count: 1
schemes:
- description: Bearer access token passed with each GraphQL request. Missing/invalid tokens yield extensions.code UNAUTHENTICATED.
  name: bearerAuth
  scheme: bearer
  sources:
  - graphql/hypercore-schema.graphql
  type: http
slug: hypercore-authentication
source_filename: hypercore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hypercore.ai/docs/api/authentication/\nverified_via: live probe of https://api.hypercore.ai/graphql\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  transport: graphql\nnotes: >-\n  Hypercore exposes a single GraphQL endpoint at https://api.hypercore.ai/graphql.\n  Authentication is by a bearer access token supplied on the request. An\n  unauthenticated request returns a GraphQL error with\n  extensions.code = \"UNAUTHENTICATED\" and message \"missing access token\". The\n  schema declares a custom `@auth` directive used to enforce authorization at the\n  field/operation level. GraphQL introspection is currently open on the production\n  endpoint (unauthenticated).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer access token passed with each GraphQL request. Missing/invalid tokens\n    yield extensions.code UNAUTHENTICATED.\n  sources:\n  - graphql/hypercore-schema.graphql\n\
  directives:\n- name: auth\n  description: Custom GraphQL directive enforcing authentication/authorization per field.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypercore/refs/heads/main/authentication/hypercore-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Loan Management
- Private Credit
- Lending
- Venture Debt
- Commercial Real Estate
- Loan Servicing
- Fintech
- Financial Services
- GraphQL
---
