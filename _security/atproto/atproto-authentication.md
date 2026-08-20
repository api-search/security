---
api_key_in: []
api_specs:
- filename: atproto-actor-api-openapi.yml
  format: yaml
  label: AT Protocol actor API
  slug: atproto-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-actor-api-openapi.yml
- filename: atproto-feed-api-openapi.yml
  format: yaml
  label: AT Protocol feed API
  slug: atproto-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-feed-api-openapi.yml
- filename: atproto-graph-api-openapi.yml
  format: yaml
  label: AT Protocol graph API
  slug: atproto-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-graph-api-openapi.yml
- filename: atproto-identity-api-openapi.yml
  format: yaml
  label: AT Protocol identity API
  slug: atproto-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-identity-api-openapi.yml
- filename: atproto-notification-api-openapi.yml
  format: yaml
  label: AT Protocol notification API
  slug: atproto-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-notification-api-openapi.yml
- filename: atproto-repo-api-openapi.yml
  format: yaml
  label: AT Protocol repo API
  slug: atproto-repo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-repo-api-openapi.yml
- filename: atproto-server-api-openapi.yml
  format: yaml
  label: AT Protocol server API
  slug: atproto-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-server-api-openapi.yml
- filename: atproto-sync-api-openapi.yml
  format: yaml
  label: AT Protocol sync API
  slug: atproto-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-sync-api-openapi.yml
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
- Open-Source
- Bluesky
- Fediverse
- Identity
- XRPC
- Lexicon
---
