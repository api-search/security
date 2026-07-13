---
api_key_in:
- query
api_specs:
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Channels API
  slug: getstream-chat-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Messages API
  slug: getstream-chat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Members API
  slug: getstream-chat-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Reactions API
  slug: getstream-chat-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Threads API
  slug: getstream-chat-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Users API
  slug: getstream-chat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Devices and Push API
  slug: getstream-chat-devices-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Moderation API
  slug: getstream-chat-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Permissions and Roles API
  slug: getstream-chat-permissions-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Campaigns API
  slug: getstream-chat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
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
- Real Time
---
