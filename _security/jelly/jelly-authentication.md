---
api_key_in: []
auth_types:
- http
description: The Jelly GraphQL API at https://api.getjelly.co.uk/ requires a bearer token. Unauthenticated operations return a GraphQL error with extensions.code = "UNAUTHENTICATED" ("Unauthorized access"). Schema introspection is publicly available; all data/mutation operations are authenticated. Tokens are issued through the Jelly kitchen app (kitchen.getjelly.co.uk) sign-in; Jelly does not publish a public OAuth authorization server or developer API-key console.
kind: authentication
layout: security
method: searched
name: Jelly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jelly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jelly
provider_slug: jelly
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Authorization: Bearer <token> header required on all authenticated GraphQL operations. Observed live: omitting it yields {"extensions":{"code":"UNAUTHENTICATED"}}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api.getjelly.co.uk/
  type: http
slug: jelly-authentication
source_filename: jelly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.getjelly.co.uk/\ndescription: >-\n  The Jelly GraphQL API at https://api.getjelly.co.uk/ requires a bearer token.\n  Unauthenticated operations return a GraphQL error with\n  extensions.code = \"UNAUTHENTICATED\" (\"Unauthorized access\"). Schema\n  introspection is publicly available; all data/mutation operations are\n  authenticated. Tokens are issued through the Jelly kitchen app\n  (kitchen.getjelly.co.uk) sign-in; Jelly does not publish a public OAuth\n  authorization server or developer API-key console.\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Authorization: Bearer <token> header required on all authenticated\n      GraphQL operations. Observed live: omitting it yields\n      {\"extensions\":{\"code\":\"UNAUTHENTICATED\"}}.\n    sources: [https://api.getjelly.co.uk/]\n\
  transport:\n  protocol: graphql\n  endpoint: https://api.getjelly.co.uk/\n  method: POST\nroles:\n  # from the UserRole enum in the GraphQL schema\n  - admin\n  - kitchen\nnotes: >-\n  This profile is searched from live API behaviour rather than an OpenAPI\n  securitySchemes block (Jelly ships a GraphQL API, not OpenAPI). No public\n  self-serve API credential page was found; access is scoped to authenticated\n  kitchen-app sessions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jelly/refs/heads/main/authentication/jelly-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Hospitality
- Restaurants
- Kitchen Management
- Food Costing
- Recipe Costing
- Invoice Processing
- GraphQL
- SaaS
---
