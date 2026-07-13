---
api_key_in: []
api_specs:
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Authentication API
  slug: nakama-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Account API
  slug: nakama-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Friends and Groups API
  slug: nakama-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Storage API
  slug: nakama-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Leaderboards and Tournaments API
  slug: nakama-leaderboards-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Notifications API
  slug: nakama-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama RPC and Runtime API
  slug: nakama-rpc-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-asyncapi.yml
  format: yaml
  label: Nakama Realtime Socket API
  slug: nakama-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/asyncapi/nakama-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nakama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nakama secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nakama
provider_slug: nakama
scheme_count: 2
schemes:
- description: HTTP Basic auth using the server key as the username and an empty password. Guards the authenticate endpoints.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/nakama-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'The JWT session token returned by an authenticate call, sent as `Authorization: Bearer <session_token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nakama-openapi.yml
  type: http
slug: nakama-authentication
source_filename: nakama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nakama-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using the server key as the username and an empty password. Guards\n    the authenticate endpoints.\n  sources:\n  - openapi/nakama-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'The JWT session token returned by an authenticate call, sent as `Authorization:\n    Bearer <session_token>`.'\n  sources:\n  - openapi/nakama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/authentication/nakama-authentication.yml
summary_line: http · 2 schemes
tags:
- Gaming
- Game Backend
- Backend
- Realtime
- Multiplayer
- Matchmaking
- Leaderboards
- Social
- Open Source
---
