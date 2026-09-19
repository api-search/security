---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: getstream-product-chat-api-openapi.yml
  format: yaml
  label: Stream Product:chat API
  slug: getstream-product-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-product-chat-api-openapi.yml
- filename: getstream-product-common-api-openapi.yml
  format: yaml
  label: Stream Product:common API
  slug: getstream-product-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-product-common-api-openapi.yml
- filename: getstream-product-feeds-api-openapi.yml
  format: yaml
  label: Stream Product:feeds API
  slug: getstream-product-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-product-feeds-api-openapi.yml
- filename: getstream-product-moderation-api-openapi.yml
  format: yaml
  label: Stream Product:moderation API
  slug: getstream-product-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-product-moderation-api-openapi.yml
- filename: getstream-product-video-api-openapi.yml
  format: yaml
  label: Stream Product:video API
  slug: getstream-product-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-product-video-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Getstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stream secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stream
provider_slug: getstream
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'A Stream JWT sent in the `Authorization` header. Server-side tokens omit the `user_id` claim; a `Stream-Auth-Type: jwt` header must accompany the request.'
  name: JWT
  scheme: bearer
  sources:
  - openapi/getstream-openapi.yml
  type: http
- description: The application API key, sent as the `api_key` query parameter on every request.
  in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/getstream-openapi.yml
  type: apiKey
slug: getstream-authentication
source_filename: getstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/getstream-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'A Stream JWT sent in the `Authorization` header. Server-side tokens omit the\n    `user_id` claim; a `Stream-Auth-Type: jwt` header must accompany the request.'\n  sources:\n  - openapi/getstream-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: The application API key, sent as the `api_key` query parameter on every request.\n  sources:\n  - openapi/getstream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/authentication/getstream-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Chat
- Messaging
- Activity Feeds
- Video
- Audio
- Moderation
- WebSocket
- Real-Time
---
