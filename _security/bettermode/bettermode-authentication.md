---
api_key_in: []
auth_types:
- http
description: 'Bettermode''s GraphQL API is authenticated with bearer access tokens passed on the Authorization header. Two token classes are documented: App Access Tokens (for installed apps acting server-to-server) and Member Access Tokens (acting as a specific community member). Guest tokens grant limited unauthenticated read access. There are no API keys or scopes in the classic OAuth sense; an app''s reach is bounded by the communities it is installed on and the permissions granted at install time.'
kind: authentication
layout: security
method: searched
name: Bettermode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bettermode secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bettermode
provider_slug: bettermode
scheme_count: 3
schemes:
- description: Issued to a Bettermode App; authenticates server-to-server requests. Scoped to the communities the app is installed on. Managed from the developer portal (app credentials).
  name: AppAccessToken
  scheme: bearer
  sources:
  - https://developers.bettermode.com/docs/guide/apps/getting-started/
  type: http
- description: Authenticates requests as a specific community member; obtained through the token/login GraphQL operations. Reflects that member's permissions.
  name: MemberAccessToken
  scheme: bearer
  sources:
  - https://developers.bettermode.com/docs/guide/graphql/getting-started/
  type: http
- description: Limited token for unauthenticated (guest) access to public read operations.
  name: GuestToken
  scheme: bearer
  sources:
  - https://developers.bettermode.com/docs/guide/graphql/getting-started/
  type: http
slug: bettermode-authentication
source_filename: bettermode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.bettermode.com/docs/guide/graphql/getting-started/\ndocs: https://developers.bettermode.com/docs/guide/\ndescription: >-\n  Bettermode's GraphQL API is authenticated with bearer access tokens passed on\n  the Authorization header. Two token classes are documented: App Access Tokens\n  (for installed apps acting server-to-server) and Member Access Tokens (acting\n  as a specific community member). Guest tokens grant limited unauthenticated\n  read access. There are no API keys or scopes in the classic OAuth sense; an\n  app's reach is bounded by the communities it is installed on and the\n  permissions granted at install time.\nsummary:\n  types: [http]\n  scheme: bearer\n  token_classes: [App Access Token, Member Access Token, Guest Token]\n  transport: Authorization header\nschemes:\n  - name: AppAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      Issued to a Bettermode App; authenticates\
  \ server-to-server requests. Scoped\n      to the communities the app is installed on. Managed from the developer\n      portal (app credentials).\n    sources: [https://developers.bettermode.com/docs/guide/apps/getting-started/]\n  - name: MemberAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      Authenticates requests as a specific community member; obtained through the\n      token/login GraphQL operations. Reflects that member's permissions.\n    sources: [https://developers.bettermode.com/docs/guide/graphql/getting-started/]\n  - name: GuestToken\n    type: http\n    scheme: bearer\n    description: >-\n      Limited token for unauthenticated (guest) access to public read operations.\n    sources: [https://developers.bettermode.com/docs/guide/graphql/getting-started/]\nendpoints:\n  us: https://api.bettermode.com\n  eu: https://api.bettermode.de\nnotes: >-\n  All GraphQL requests are HTTP POST to the region endpoint with the bearer token\n  on the Authorization\
  \ header. Apps are created and their credentials managed in\n  the developer portal (app.bettermode.com/portal); an app must have an owner\n  community and the creator must be an admin of at least one community.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettermode/refs/heads/main/authentication/bettermode-authentication.yml
summary_line: http · 3 schemes
tags:
- Community
- Customer Community
- Community Platform
- Customer Engagement
- Customer Success
- GraphQL
- Webhooks
- No-Code
- SaaS
- Developer
---
