---
api_key_in: []
auth_types:
- bearer-session
description: ''
kind: authentication
layout: security
method: derived
name: Brigad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brigad secures its APIs with bearer-session across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brigad
provider_slug: brigad
scheme_count: 1
schemes:
- description: End-user session/bearer token minted by the Brigad app login flow, sent to the GraphQL routers. No public client-credentials or API-key path is documented or offered to third parties.
  name: BrigadUserSession
  scheme: bearer
  sources:
  - graphql/brigad-talent.graphql
  - graphql/brigad-agent.graphql
  - graphql/brigad-legacy.graphql
  type: http
slug: brigad-authentication
source_filename: brigad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: graphql/brigad-talent.graphql, graphql/brigad-agent.graphql, graphql/brigad-legacy.graphql\nnote: >-\n  Brigad publishes no auth documentation (no developer program). This profile is\n  derived from observed behaviour of the first-party GraphQL routers. Anonymous\n  __schema introspection is OPEN on all three routers, but data queries and every\n  mutation require an authenticated end-user session established by the Brigad web\n  app (app.hsp.brigad.co) / mobile apps. No OpenAPI securitySchemes exist to run\n  derive-authentication.py against; no OAuth authorization-server / OIDC discovery\n  document is served (see well-known/brigad-well-known.yml). Not a third-party\n  developer credential surface.\nsummary:\n  types: [bearer-session]\n  api_key_in: []\n  oauth2_flows: []\n  introspection: open-anonymous\nschemes:\n- name: BrigadUserSession\n  type: http\n  scheme: bearer\n  description: >-\n    End-user session/bearer token\
  \ minted by the Brigad app login flow, sent to\n    the GraphQL routers. No public client-credentials or API-key path is\n    documented or offered to third parties.\n  sources:\n  - graphql/brigad-talent.graphql\n  - graphql/brigad-agent.graphql\n  - graphql/brigad-legacy.graphql\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brigad/refs/heads/main/authentication/brigad-authentication.yml
summary_line: bearer-session · 1 scheme
tags:
- Company
- Staffing
- Marketplace
- Hospitality
- Healthcare
- Gig Economy
- Freelance
- Workforce
---
