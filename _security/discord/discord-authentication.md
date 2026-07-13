---
api_key_in:
- header
api_specs:
- filename: discord-api-spec
  format: yaml
  label: Discord REST API
  slug: discord-rest-api
  spec_type: OpenAPI
  url: https://github.com/discord/discord-api-spec
- filename: discord-gateway-api-asyncapi.yml
  format: yaml
  label: Discord Gateway API
  slug: discord-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/asyncapi/discord-gateway-api-asyncapi.yml
- filename: discord-interactions-api-openapi.yml
  format: yaml
  label: Discord Interactions API
  slug: discord-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-interactions-api-openapi.yml
- filename: discord-oauth2-api-openapi.yml
  format: yaml
  label: Discord OAuth2 API
  slug: discord-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-oauth2-api-openapi.yml
- filename: discord-webhook-events-api-openapi.yml
  format: yaml
  label: Discord Webhook Events API
  slug: discord-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-webhook-events-api-openapi.yml
- filename: discord-voice-api-asyncapi.yml
  format: yaml
  label: Discord Voice API
  slug: discord-voice-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/asyncapi/discord-voice-api-asyncapi.yml
- filename: discord-linked-roles-api-openapi.yml
  format: yaml
  label: Discord Linked Roles API
  slug: discord-linked-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-linked-roles-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Discord Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Discord secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Discord
provider_slug: discord
scheme_count: 4
schemes:
- description: Bot token authentication
  name: BotToken
  scheme: bearer
  sources:
  - openapi/discord-interactions-api-openapi.yml
  - openapi/discord-linked-roles-api-openapi.yml
  - openapi/discord-oauth2-api-openapi.yml
  - openapi/discord-rest-api-openapi.yml
  type: http
- description: Discord bot token
  in: header
  name: BotToken
  parameter: Authorization
  sources:
  - openapi/discord-openapi-original.yml
  type: apiKey
- flows:
  - authorizationUrl: discord.com/oauth2/authorize
    flow: implicit
    scopes: 31
  - flow: clientCredentials
    scopes: 32
    tokenUrl: https://discord.com/api/oauth2/token
  - authorizationUrl: discord.com/oauth2/authorize
    flow: authorizationCode
    scopes: 32
    tokenUrl: https://discord.com/api/oauth2/token
  name: OAuth2
  sources:
  - openapi/discord-openapi-original.yml
  type: oauth2
- flows:
  - authorizationUrl: https://discord.com/oauth2/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://discord.com/api/v10/oauth2/token
  name: OAuth2
  sources:
  - openapi/discord-rest-api-openapi.yml
  type: oauth2
slug: discord-authentication
source_filename: discord-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/discord-interactions-api-openapi.yml, openapi/discord-linked-roles-api-openapi.yml,\n  openapi/discord-oauth2-api-openapi.yml, openapi/discord-openapi-original.yml, openapi/discord-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: BotToken\n  type: http\n  scheme: bearer\n  description: Bot token authentication\n  sources:\n  - openapi/discord-interactions-api-openapi.yml\n  - openapi/discord-linked-roles-api-openapi.yml\n  - openapi/discord-oauth2-api-openapi.yml\n  - openapi/discord-rest-api-openapi.yml\n- name: BotToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Discord bot token\n  sources:\n  - openapi/discord-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: discord.com/oauth2/authorize\n\
  \    scopes: 31\n  - flow: clientCredentials\n    tokenUrl: https://discord.com/api/oauth2/token\n    scopes: 32\n  - flow: authorizationCode\n    authorizationUrl: discord.com/oauth2/authorize\n    tokenUrl: https://discord.com/api/oauth2/token\n    scopes: 32\n  sources:\n  - openapi/discord-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discord.com/oauth2/authorize\n    tokenUrl: https://discord.com/api/v10/oauth2/token\n    scopes: 8\n  sources:\n  - openapi/discord-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/authentication/discord-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
---
