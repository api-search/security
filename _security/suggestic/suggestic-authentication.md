---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Suggestic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suggestic secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Suggestic
provider_slug: suggestic
scheme_count: 2
schemes:
- companion_headers:
  - description: User UUID the request operates "on behalf of" (e.g. ffffe9fa-3b49-4050-80d1-06129a722d0b). Not required for open mutations like createUser/loginUser or queries marked with `*`.
    name: sg-user
    required: false
  - description: Partner slug for clients with an isolated database; used in place of sg-user for partner-scoped authentication.
    name: Suggestic-Partner
    required: false
  context: server-side
  description: 'Static API token issued to the developer/partner. Sent as the `Authorization: Token <token>` header. Requires a companion `sg-user` header carrying the user UUID the request acts on behalf of. Do NOT use on the client side.'
  format: Token <api_token>
  in: header
  name: apiTokenAuth
  parameter_name: Authorization
  type: apiKey
- bearerFormat: JWT
  context: client-side
  description: 'JWT issued to an end user. Obtained by POST to https://production.suggestic.com/api/v1/login with email+password, or via the `login(userId:)` mutation from a trusted backend using the API token. Sent as `Authorization: Bearer <jwt>`. When a JWT is used, the sg-user header is not required. Access tokens expire after 2 hours; a refresh_token (from the login mutation) renews them.'
  name: jwtBearerAuth
  refresh_supported: true
  scheme: bearer
  token_endpoint: https://production.suggestic.com/api/v1/login
  token_ttl_seconds: 7200
  type: http
slug: suggestic-authentication
source_filename: suggestic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.suggestic.com/graphql/graphql/authentication.md\ndocs: https://docs.suggestic.com/graphql/graphql/authentication\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  notes: >-\n    Suggestic's GraphQL API supports two authentication methods. JWT (Bearer)\n    for client-side apps, and a static API Token plus sg-user header for\n    server-side apps acting on behalf of a user. There is no OAuth2 scope\n    surface, so no scopes/ artifact is emitted.\nschemes:\n  - name: apiTokenAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: \"Token <api_token>\"\n    context: server-side\n    description: >-\n      Static API token issued to the developer/partner. Sent as the\n      `Authorization: Token <token>` header. Requires a companion `sg-user`\n      header carrying the user UUID the request acts on behalf of. Do NOT use\n    \
  \  on the client side.\n    companion_headers:\n      - name: sg-user\n        required: false\n        description: >-\n          User UUID the request operates \"on behalf of\" (e.g.\n          ffffe9fa-3b49-4050-80d1-06129a722d0b). Not required for open\n          mutations like createUser/loginUser or queries marked with `*`.\n      - name: Suggestic-Partner\n        required: false\n        description: >-\n          Partner slug for clients with an isolated database; used in place of\n          sg-user for partner-scoped authentication.\n  - name: jwtBearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    context: client-side\n    description: >-\n      JWT issued to an end user. Obtained by POST to\n      https://production.suggestic.com/api/v1/login with email+password, or via\n      the `login(userId:)` mutation from a trusted backend using the API token.\n      Sent as `Authorization: Bearer <jwt>`. When a JWT is used, the sg-user\n      header is not required.\
  \ Access tokens expire after 2 hours; a\n      refresh_token (from the login mutation) renews them.\n    token_endpoint: https://production.suggestic.com/api/v1/login\n    token_ttl_seconds: 7200\n    refresh_supported: true\nenvironments:\n  production: https://production.suggestic.com/graphql\n  staging: https://staging.suggestic.com/graphql\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suggestic/refs/heads/main/authentication/suggestic-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Nutrition
- Health
- Meal Planning
- Recipes
- Food
- GraphQL
- Personalization
- Wellness
- Telehealth
- Artificial Intelligence
---
