---
api_key_in: []
api_specs:
- filename: livechat-openapi.yml
  format: yaml
  label: LiveChat Agent Chat API
  slug: agent-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/openapi/livechat-openapi.yml
- filename: livechat-asyncapi.yml
  format: yaml
  label: LiveChat Webhooks and RTM API
  slug: webhooks-and-rtm
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/openapi/livechat-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Livechat Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveChat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LiveChat
provider_slug: livechat
scheme_count: 1
schemes:
- description: OAuth 2.x bearer token or Personal Access Token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/livechat-openapi.yml
  type: http
slug: livechat-authentication
source_filename: livechat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/livechat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.x bearer token or Personal Access Token.\n  sources:\n  - openapi/livechat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/authentication/livechat-authentication.yml
summary_line: http · 1 scheme
tags:
- Live Chat
- Customer Service
- Customer Support
- Messaging
- Sales
- Help Desk
---
