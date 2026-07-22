---
api_key_in:
- query
- sdk-init
api_specs:
- filename: sanas-stream-asyncapi.yml
  format: yaml
  label: Sanas Stream API
  slug: sanas-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanas/refs/heads/main/asyncapi/sanas-stream-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sanas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sanas secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sanas
provider_slug: sanas
scheme_count: 3
schemes:
- applies_to: Sanas Stream API (WebSocket)
  description: API key issued from the Sanas Developer Console, supplied as the api_key query parameter on the wss://api.sanaslt.com/v3/stream connection URL. Validated before the WebSocket upgrade; failure returns HTTP 401.
  in: query
  name: apiKey
  parameter: api_key
  type: apiKey
- applies_to: Sanas Stream API (WebSocket)
  bearer_format: JWT
  description: JWT bearer token (issued via Supabase) supplied as the token query parameter. Provide either token or api_key, not both.
  in: query
  name: bearerToken
  parameter: token
  scheme: bearer
  type: http
- applies_to: Sanas Speech AI SDK (C++/Python)
  description: API key from the Sanas Developer Console set on InitParams.apiKey (or read from the SANAS_API_KEY environment variable) at SDK Initialize(). The SDK uses it to authenticate to Sanas Cloud and auto-resolve the server endpoint.
  in: sdk-init
  name: sdkApiKey
  parameter: InitParams.apiKey
  type: apiKey
slug: sanas-authentication
source_filename: sanas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.sanas.ai/Docs/Language-Translation/WebSocket-API.md\ndocs: https://developer.sanas.ai/API-Reference/Cpp-SDK/Guides/Installation.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  - sdk-init\n  http_schemes:\n  - bearer\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: Sanas Stream API (WebSocket)\n  description: >-\n    API key issued from the Sanas Developer Console, supplied as the api_key\n    query parameter on the wss://api.sanaslt.com/v3/stream connection URL.\n    Validated before the WebSocket upgrade; failure returns HTTP 401.\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: query\n  parameter: token\n  applies_to: Sanas Stream API (WebSocket)\n  description: >-\n    JWT bearer token (issued via Supabase) supplied as the token query\n    parameter. Provide either token or api_key,\
  \ not both.\n- name: sdkApiKey\n  type: apiKey\n  in: sdk-init\n  parameter: InitParams.apiKey\n  applies_to: Sanas Speech AI SDK (C++/Python)\n  description: >-\n    API key from the Sanas Developer Console set on InitParams.apiKey (or read\n    from the SANAS_API_KEY environment variable) at SDK Initialize(). The SDK\n    uses it to authenticate to Sanas Cloud and auto-resolve the server endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanas/refs/heads/main/authentication/sanas-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Speech AI
- Voice AI
- Accent Translation
- Language Translation
- Speech Enhancement
- Real-Time Audio
- SDK
- WebSocket
- Contact Center
---
