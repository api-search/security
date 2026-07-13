---
api_key_in:
- header
- query
api_specs:
- filename: stream-io-chat-openapi.yml
  format: yaml
  label: Stream Chat API
  slug: chat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-chat-openapi.yml
- filename: stream-io-video-openapi.yml
  format: yaml
  label: Stream Video & Audio API
  slug: video
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-video-openapi.yml
- filename: stream-io-moderation-openapi.yml
  format: yaml
  label: Stream Moderation API
  slug: moderation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-moderation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stream Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stream secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stream
provider_slug: stream-io
scheme_count: 3
schemes:
- description: 'JWT should be always provided when stream-auth-type=jwt.


    Using JWT auth request could be authenticated as user or as server-side.


    When using user authentication permission checking is going to be applied to requests based on the user that is

    performing a request.


    The `authorization` header should be a JWT string signed using the secret attached to the API key used to perform

    requests.


    **WARNIN'
  in: header
  name: JWT
  parameter: Authorization
  sources:
  - openapi/stream-io-chat-openapi.yml
  - openapi/stream-io-moderation-openapi.yml
  - openapi/stream-io-serverside-openapi.yml
  - openapi/stream-io-video-openapi.yml
  type: apiKey
- description: Application API key should be always set in order to authenticate the request.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/stream-io-chat-openapi.yml
  - openapi/stream-io-moderation-openapi.yml
  - openapi/stream-io-serverside-openapi.yml
  - openapi/stream-io-video-openapi.yml
  type: apiKey
- description: 'Stream-Auth-Type should be always set in order to authenticate the request. Possible

    values: `jwt` or `anonymous`.


    `jwt` allows you to authenticate as a user. With this auth type you should also provide valid JWT in Authorization

    header.


    `anonymous` allows you to authenticate as anonymous user. Please note that most advanced features are not available

    to anonymous users.'
  in: header
  name: stream-auth-type
  parameter: Stream-Auth-Type
  sources:
  - openapi/stream-io-chat-openapi.yml
  - openapi/stream-io-moderation-openapi.yml
  - openapi/stream-io-serverside-openapi.yml
  - openapi/stream-io-video-openapi.yml
  type: apiKey
slug: stream-io-authentication
source_filename: stream-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stream-io-chat-openapi.yml, openapi/stream-io-moderation-openapi.yml, openapi/stream-io-serverside-openapi.yml,\n  openapi/stream-io-video-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    JWT should be always provided when stream-auth-type=jwt.\n\n    Using JWT auth request could be authenticated as user or as server-side.\n\n    When using user authentication permission checking is going to be applied to requests based on the user that is\n    performing a request.\n\n    The `authorization` header should be a JWT string signed using the secret attached to the API key used to perform\n    requests.\n\n    **WARNIN\n  sources:\n  - openapi/stream-io-chat-openapi.yml\n  - openapi/stream-io-moderation-openapi.yml\n  - openapi/stream-io-serverside-openapi.yml\n  - openapi/stream-io-video-openapi.yml\n\
  - name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Application API key should be always set in order to authenticate the request.\n  sources:\n  - openapi/stream-io-chat-openapi.yml\n  - openapi/stream-io-moderation-openapi.yml\n  - openapi/stream-io-serverside-openapi.yml\n  - openapi/stream-io-video-openapi.yml\n- name: stream-auth-type\n  type: apiKey\n  in: header\n  parameter: Stream-Auth-Type\n  description: |-\n    Stream-Auth-Type should be always set in order to authenticate the request. Possible\n    values: `jwt` or `anonymous`.\n\n    `jwt` allows you to authenticate as a user. With this auth type you should also provide valid JWT in Authorization\n    header.\n\n    `anonymous` allows you to authenticate as anonymous user. Please note that most advanced features are not available\n    to anonymous users.\n  sources:\n  - openapi/stream-io-chat-openapi.yml\n  - openapi/stream-io-moderation-openapi.yml\n  - openapi/stream-io-serverside-openapi.yml\n\
  \  - openapi/stream-io-video-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/authentication/stream-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Realtime
- Chat
- Messaging
- Video
- Audio
- Activity Feeds
- Moderation
- SDK
---
