---
api_key_in: []
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Snapser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snapser secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snapser
provider_slug: snapser
scheme_count: 2
schemes:
- delivery:
  - command-line arg --api-key
  - env var SNAPSER_API_KEY
  - config file ~/.snapser/config
  limit: up to 3 API keys per user account
  name: personalApiKey
  plane: developer-management
  type: apiKey
  used_by:
  - snapctl CLI
  - dashboard
- connectors:
  - anon
  - apple
  - discord
  - email
  - google
  - steam
  - xbox
  description: The Authentication Snap issues a Snapser session token to end users after verifying an identity connector. The token is then presented to the Snapend gateway on subsequent API calls.
  name: authSnapConnectors
  plane: application-runtime
  type: oauth2/identity-provider
slug: snapser-authentication
source_filename: snapser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.snapser.com/docs/infra/snaps/auth/connectors\ndocs:\n- https://docs.snapser.com/docs/infra/snaps/auth/connectors\n- https://docs.snapser.com/docs/infra/snaps/auth/config-tools/api-key-manager\nnotes: >-\n  Snapser has no single public OpenAPI to derive securitySchemes from — each\n  customer deploys a Snapend with its own API gateway. This profile is captured\n  from the public documentation surface. Two distinct auth planes exist: (1) the\n  developer/management plane driven by a personal API key (used by the snapctl\n  CLI and dashboard); and (2) the runtime application plane where end users of a\n  game/app authenticate through the Authentication Snap's connectors and receive\n  a session token used against the Snapend gateway.\nsummary:\n  types: [apiKey, oauth2]\n  planes: [developer-management, application-runtime]\nschemes:\n- name: personalApiKey\n  plane: developer-management\n  type: apiKey\n  used_by:\
  \ [snapctl CLI, dashboard]\n  delivery:\n  - command-line arg --api-key\n  - env var SNAPSER_API_KEY\n  - config file ~/.snapser/config\n  limit: up to 3 API keys per user account\n- name: authSnapConnectors\n  plane: application-runtime\n  type: oauth2/identity-provider\n  description: >-\n    The Authentication Snap issues a Snapser session token to end users after\n    verifying an identity connector. The token is then presented to the Snapend\n    gateway on subsequent API calls.\n  connectors:\n  - anon\n  - apple\n  - discord\n  - email\n  - google\n  - steam\n  - xbox\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapser/refs/heads/main/authentication/snapser-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Game Development
- Backend as a Service
- Game Backend
- Authentication
- Leaderboards
- Multiplayer
- Microservices
- SDK Generation
- Developer Tools
---
