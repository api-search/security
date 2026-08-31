---
api_key_in: []
auth_types:
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Looking Glass Factory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Looking Glass Factory secures its APIs with oauth2 and none across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Looking Glass Factory
provider_slug: looking-glass-factory
scheme_count: 2
schemes:
- applies_to: Blocks GraphQL API (https://blocks.glass/api/graphql)
  detail: '"Blocks uses Auth0 under the hood for authentication." Developers request a Client ID via form; blocks.js runs the OAuth redirect login and attaches the resulting bearer token to GraphQL requests.'
  flow: authorizationCode
  name: Auth0 (Blocks API)
  provider: Auth0
  source: https://github.com/Looking-Glass/blocks.js
  type: oauth2
- applies_to: Bridge HTTP REST API (localhost media-player control)
  detail: The Bridge REST API is exposed by the locally-installed Looking Glass Bridge runtime over loopback; it controls the local media player and carries no authentication.
  name: None (Bridge local REST)
  source: https://lfdocs.lookingglassfactory.com/software/looking-glass-bridge-sdk/web-application-integration
  type: none
slug: looking-glass-factory-authentication
source_filename: looking-glass-factory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/Looking-Glass/blocks.js + https://lfdocs.lookingglassfactory.com/software/looking-glass-bridge-sdk/web-application-integration\ndocs: https://docs.lookingglassfactory.com/\nsummary:\n  types: [oauth2, none]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Looking Glass exposes two developer APIs with distinct auth models. The\n    hosted Blocks GraphQL API authenticates via Auth0 (OAuth 2.0 / OIDC,\n    redirect-based authorization-code login using a per-app Client ID). The\n    local Bridge HTTP REST API is served by the Looking Glass Bridge desktop\n    runtime on localhost and requires no network credential (loopback-only).\nschemes:\n  - name: Auth0 (Blocks API)\n    type: oauth2\n    flow: authorizationCode\n    provider: Auth0\n    applies_to: Blocks GraphQL API (https://blocks.glass/api/graphql)\n    detail: >-\n      \"Blocks uses Auth0 under the hood for authentication.\" Developers request\n\
  \      a Client ID via form; blocks.js runs the OAuth redirect login and attaches\n      the resulting bearer token to GraphQL requests.\n    source: https://github.com/Looking-Glass/blocks.js\n  - name: None (Bridge local REST)\n    type: none\n    applies_to: Bridge HTTP REST API (localhost media-player control)\n    detail: >-\n      The Bridge REST API is exposed by the locally-installed Looking Glass\n      Bridge runtime over loopback; it controls the local media player and\n      carries no authentication.\n    source: https://lfdocs.lookingglassfactory.com/software/looking-glass-bridge-sdk/web-application-integration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looking-glass-factory/refs/heads/main/authentication/looking-glass-factory-authentication.yml
summary_line: oauth2/none · 2 schemes
tags:
- Company
- Hardware
- Holographic Displays
- 3D
- Light Field
- Developer Tools
- SDK
- GraphQL
- WebXR
- AR VR
---
