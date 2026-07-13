---
api_key_in: []
api_specs:
- filename: atproto-com-atproto-openapi.yml
  format: yaml
  label: AT Protocol Core API (com.atproto)
  slug: com-atproto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-com-atproto-openapi.yml
- filename: atproto-app-bsky-openapi.yml
  format: yaml
  label: Bluesky Application API (app.bsky)
  slug: app-bsky
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-app-bsky-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Atproto Authentication
name_suffix: Authentication
oauth_flows: []
overview: AT Protocol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AT Protocol
provider_slug: atproto
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Access JWT obtained from com.atproto.server.createSession
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/atproto-app-bsky-openapi.yml
  - openapi/atproto-com-atproto-openapi.yml
  type: http
slug: atproto-authentication
source_filename: atproto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atproto-app-bsky-openapi.yml, openapi/atproto-com-atproto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access JWT obtained from com.atproto.server.createSession\n  sources:\n  - openapi/atproto-app-bsky-openapi.yml\n  - openapi/atproto-com-atproto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/authentication/atproto-authentication.yml
summary_line: http · 1 scheme
tags:
- Social Networking
- Decentralized
- Federated
- Open Source
- Bluesky
- Fediverse
- Identity
- XRPC
- Lexicon
---
