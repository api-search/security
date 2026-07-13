---
api_key_in:
- query
api_specs:
- filename: pusher-asyncapi.yml
  format: yaml
  label: Pusher Channels API
  slug: channels-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pusher/refs/heads/main/asyncapi/pusher-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pusher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pusher secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pusher
provider_slug: pusher
scheme_count: 1
schemes:
- description: 'Pusher request signing. Every request must include the query

    parameters `auth_key`, `auth_timestamp` (Unix seconds),

    `auth_version=1.0`, `body_md5` (hex MD5 of the request body when

    present), and `auth_signature`. `auth_signature` is the

    HMAC-SHA256 (hex) of the canonical string

    `"<METHOD>\n<PATH>\n<SORTED_QUERY_STRING>"` using the application

    secret as the key.'
  in: query
  name: hmacAuth
  parameter: auth_signature
  sources:
  - openapi/pusher-openapi.yml
  type: apiKey
slug: pusher-authentication
source_filename: pusher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pusher-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: hmacAuth\n  type: apiKey\n  in: query\n  parameter: auth_signature\n  description: |-\n    Pusher request signing. Every request must include the query\n    parameters `auth_key`, `auth_timestamp` (Unix seconds),\n    `auth_version=1.0`, `body_md5` (hex MD5 of the request body when\n    present), and `auth_signature`. `auth_signature` is the\n    HMAC-SHA256 (hex) of the canonical string\n    `\"<METHOD>\\n<PATH>\\n<SORTED_QUERY_STRING>\"` using the application\n    secret as the key.\n  sources:\n  - openapi/pusher-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pusher/refs/heads/main/authentication/pusher-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Realtime
- WebSockets
- Pub/Sub
- Push Notifications
- Messaging
---
