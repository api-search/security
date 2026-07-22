---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Momento Authentication
name_suffix: Authentication
oauth_flows: []
overview: Momento secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Momento
provider_slug: momento
scheme_count: 2
schemes:
- description: A Momento API key (auth token) is passed in the Authorization header on HTTP requests and as gRPC `authorization` metadata. Keys are minted in the Momento Console or via the CLI/SDK and encode the Momento endpoint they are valid against.
  header: Authorization
  in: header
  name: MomentoApiKey
  sources:
  - https://docs.momentohq.com/cache/develop/api-reference/http-api
  - grpc/momento-cachepubsub.proto
  type: apiKey
- description: The HTTP API also accepts the API key as a `token` query-string parameter (e.g. `?token=<key>`), primarily for browser and edge use.
  in: query
  name: MomentoTokenQuery
  query_param: token
  sources:
  - https://docs.momentohq.com/cache/develop/api-reference/http-api
  type: apiKey
slug: momento-authentication
source_filename: momento-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.momentohq.com/platform/security/tokens\ndocs: https://docs.momentohq.com/cache/develop/authentication/api-keys\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: MomentoApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    description: >-\n      A Momento API key (auth token) is passed in the Authorization header on\n      HTTP requests and as gRPC `authorization` metadata. Keys are minted in the\n      Momento Console or via the CLI/SDK and encode the Momento endpoint they are\n      valid against.\n    sources: [https://docs.momentohq.com/cache/develop/api-reference/http-api, grpc/momento-cachepubsub.proto]\n  - name: MomentoTokenQuery\n    type: apiKey\n    in: query\n    query_param: token\n    description: >-\n      The HTTP API also accepts the API key as a `token` query-string parameter\n      (e.g. `?token=<key>`), primarily for browser\
  \ and edge use.\n    sources: [https://docs.momentohq.com/cache/develop/api-reference/http-api]\ntoken_model:\n  - kind: api-key\n    description: Long-lived (or fixed-expiry) API key generated in the console for a cell/endpoint.\n  - kind: disposable-token\n    description: >-\n      Short-lived, fine-grained token minted via the Token service\n      (GenerateDisposableToken) with an explicit `valid_for_seconds` expiry and a\n      Permissions object scoping it to specific caches/topics and read/write roles.\n      Designed for client-side (browser/mobile) use so long-lived keys never leave the server.\n    source: grpc/momento-token.proto\n    permissions: grpc/momento-permissionmessages.proto\n  - kind: refreshable-api-token\n    description: API tokens can be programmatically refreshed via the Auth service (GenerateApiToken / RefreshApiToken).\n    source: grpc/momento-auth.proto\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momento/refs/heads/main/authentication/momento-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Infrastructure
- Caching
- Serverless
- Cache
- Pub/Sub
- Messaging
- Event Bus
- Leaderboards
- Real Time
- gRPC
- Developer Tools
---
