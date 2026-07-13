---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Nakama API
  slug: nakama-api
  spec_type: OpenAPI
  url: https://heroiclabs.github.io/nakama-docs/
- filename: heroiclabs-hiro-rpc-api-openapi.yml
  format: yaml
  label: Hiro RPC API
  slug: hiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/openapi/heroiclabs-hiro-rpc-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Heroiclabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heroic Labs secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heroic Labs
provider_slug: heroiclabs
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: bearerAuthNakama
  scheme: bearer
  sources:
  - openapi/heroiclabs-hiro-rpc-api-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/heroiclabs-nakama-api-openapi.yml
  - openapi/heroiclabs-nakama-console-api-openapi.yml
  type: http
- in: header
  name: BearerJwt
  parameter: Authorization
  sources:
  - openapi/heroiclabs-nakama-api-openapi.yml
  - openapi/heroiclabs-nakama-console-api-openapi.yml
  type: apiKey
- in: header
  name: HttpKeyAuth
  parameter: http_key
  sources:
  - openapi/heroiclabs-nakama-api-openapi.yml
  type: apiKey
slug: heroiclabs-authentication
source_filename: heroiclabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heroiclabs-hiro-rpc-api-openapi.yml, openapi/heroiclabs-nakama-api-openapi.yml,\n  openapi/heroiclabs-nakama-console-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuthNakama\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/heroiclabs-hiro-rpc-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/heroiclabs-nakama-api-openapi.yml\n  - openapi/heroiclabs-nakama-console-api-openapi.yml\n- name: BearerJwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/heroiclabs-nakama-api-openapi.yml\n  - openapi/heroiclabs-nakama-console-api-openapi.yml\n- name: HttpKeyAuth\n  type: apiKey\n  in: header\n  parameter: http_key\n  sources:\n  - openapi/heroiclabs-nakama-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/authentication/heroiclabs-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Game Backend
- Multiplayer
- Real-Time
- WebSocket
- Matchmaking
- Leaderboards
- Social Gaming
- Open Source
- LiveOps
- gRPC
---
