---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mumo-chat-account-api-openapi.yml
  format: yaml
  label: mumo Account API
  slug: mumo-chat-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-account-api-openapi.yml
- filename: mumo-chat-deliberations-api-openapi.yml
  format: yaml
  label: mumo Deliberations API
  slug: mumo-chat-deliberations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-deliberations-api-openapi.yml
- filename: mumo-chat-sessions-api-openapi.yml
  format: yaml
  label: mumo Sessions API
  slug: mumo-chat-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-sessions-api-openapi.yml
- filename: mumo-chat-system-api-openapi.yml
  format: yaml
  label: mumo System API
  slug: mumo-chat-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mumo-chat/openapi/mumo-chat-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: mumo Authentication
name_suffix: Authentication
oauth_flows: []
overview: mumo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: mumo
provider_slug: mumo-chat
scheme_count: 2
schemes:
- description: 'Platform API key, sent as `Authorization: Bearer mmo_live_…`.


    Keys are minted at https://mumo.chat/settings/api-keys and always begin with the `mmo_live_` prefix. Each key is hashed at rest — copy the secret when it is created, because it is never shown again. Calls without a valid key return `401 unauthorized`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mumo-chat-openapi.yml
  type: http
- description: 'The same platform API key as `bearerAuth`, sent bare (`X-Mumo-Api-Key: mmo_live_…`, no `Bearer` prefix) for MCP gateways and proxies that reserve the `Authorization` header for their own use.


    Send one or the other. If both arrive, a platform key in `Authorization` takes precedence; otherwise the key in `X-Mumo-Api-Key` does, so a gateway-injected `Authorization` token cannot shadow it. Any non-ke'
  in: header
  name: apiKeyHeader
  parameter: X-Mumo-Api-Key
  sources:
  - openapi/mumo-chat-openapi.yml
  type: apiKey
slug: mumo-chat-authentication
source_filename: mumo-chat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mumo-chat-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Platform API key, sent as `Authorization: Bearer mmo_live_…`.\n\n    Keys are minted at https://mumo.chat/settings/api-keys and always begin with the `mmo_live_` prefix. Each key is hashed at rest — copy the secret when it is created, because it is never shown again. Calls without a valid key return `401 unauthorized`.\n  sources:\n  - openapi/mumo-chat-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Mumo-Api-Key\n  description: |-\n    The same platform API key as `bearerAuth`, sent bare (`X-Mumo-Api-Key: mmo_live_…`, no `Bearer` prefix) for MCP gateways and proxies that reserve the `Authorization` header for their own use.\n\n    Send one or the other. If both arrive, a platform key in `Authorization` takes precedence;\
  \ otherwise the key in `X-Mumo-Api-Key` does, so a gateway-injected `Authorization` token cannot shadow it. Any non-ke\n  sources:\n  - openapi/mumo-chat-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mumo-chat/authentication/mumo-chat-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Chatbots
- Multi-Model
- Collaboration
- OpenAI
---
