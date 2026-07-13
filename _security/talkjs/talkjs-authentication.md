---
api_key_in: []
api_specs:
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Users API
  slug: talkjs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Conversations & Participants API
  slug: talkjs-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Messages API
  slug: talkjs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Import API
  slug: talkjs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Talkjs Authentication
name_suffix: Authentication
oauth_flows: []
overview: TalkJS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TalkJS
provider_slug: talkjs
scheme_count: 1
schemes:
- description: 'A TalkJS secret key or a short-lived JWT with admin claims, sent as "Authorization: Bearer <token>".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/talkjs-openapi.yml
  type: http
slug: talkjs-authentication
source_filename: talkjs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talkjs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A TalkJS secret key or a short-lived JWT with admin claims, sent as \"Authorization:\n    Bearer <token>\".'\n  sources:\n  - openapi/talkjs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/authentication/talkjs-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat
- Messaging
- Communication
- SDK
- Webhooks
---
