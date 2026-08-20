---
api_key_in:
- query
api_specs:
- filename: getstream-application-api-openapi.yml
  format: yaml
  label: Stream Application API
  slug: getstream-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-application-api-openapi.yml
- filename: getstream-campaigns-api-openapi.yml
  format: yaml
  label: Stream Campaigns API
  slug: getstream-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-campaigns-api-openapi.yml
- filename: getstream-channels-api-openapi.yml
  format: yaml
  label: Stream Channels API
  slug: getstream-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-channels-api-openapi.yml
- filename: getstream-devices-api-openapi.yml
  format: yaml
  label: Stream Devices API
  slug: getstream-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-devices-api-openapi.yml
- filename: getstream-members-api-openapi.yml
  format: yaml
  label: Stream Members API
  slug: getstream-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-members-api-openapi.yml
- filename: getstream-messages-api-openapi.yml
  format: yaml
  label: Stream Messages API
  slug: getstream-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-messages-api-openapi.yml
- filename: getstream-moderation-api-openapi.yml
  format: yaml
  label: Stream Moderation API
  slug: getstream-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-moderation-api-openapi.yml
- filename: getstream-permissions-api-openapi.yml
  format: yaml
  label: Stream Permissions API
  slug: getstream-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-permissions-api-openapi.yml
- filename: getstream-reactions-api-openapi.yml
  format: yaml
  label: Stream Reactions API
  slug: getstream-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-reactions-api-openapi.yml
- filename: getstream-roles-api-openapi.yml
  format: yaml
  label: Stream Roles API
  slug: getstream-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-roles-api-openapi.yml
- filename: getstream-threads-api-openapi.yml
  format: yaml
  label: Stream Threads API
  slug: getstream-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-threads-api-openapi.yml
- filename: getstream-users-api-openapi.yml
  format: yaml
  label: Stream Users API
  slug: getstream-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-users-api-openapi.yml
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
- Real-Time
---
