---
api_key_in:
- path
api_specs:
- filename: telegram-bot-info-api-openapi.yml
  format: yaml
  label: Telegram Bot Info API
  slug: telegram-bot-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-bot-info-api-openapi.yml
- filename: telegram-chat-management-api-openapi.yml
  format: yaml
  label: Telegram Chat Management API
  slug: telegram-chat-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-chat-management-api-openapi.yml
- filename: telegram-getting-updates-api-openapi.yml
  format: yaml
  label: Telegram Getting Updates API
  slug: telegram-getting-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-getting-updates-api-openapi.yml
- filename: telegram-invites-api-openapi.yml
  format: yaml
  label: Telegram Invites API
  slug: telegram-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-invites-api-openapi.yml
- filename: telegram-member-management-api-openapi.yml
  format: yaml
  label: Telegram Member Management API
  slug: telegram-member-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-member-management-api-openapi.yml
- filename: telegram-message-editing-api-openapi.yml
  format: yaml
  label: Telegram Message Editing API
  slug: telegram-message-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-message-editing-api-openapi.yml
- filename: telegram-messaging-api-openapi.yml
  format: yaml
  label: Telegram Messaging API
  slug: telegram-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-messaging-api-openapi.yml
- filename: telegram-payments-api-openapi.yml
  format: yaml
  label: Telegram Payments API
  slug: telegram-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-payments-api-openapi.yml
- filename: telegram-stickers-api-openapi.yml
  format: yaml
  label: Telegram Stickers API
  slug: telegram-stickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-stickers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Telegram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telegram secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telegram
provider_slug: telegram
scheme_count: 1
schemes:
- description: Bot authentication token obtained from @BotFather (embedded in URL path)
  in: path
  name: BotToken
  parameter: token
  sources:
  - openapi/telegram-bot-openapi.yml
  type: apiKey
slug: telegram-authentication
source_filename: telegram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telegram-bot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: BotToken\n  type: apiKey\n  in: path\n  parameter: token\n  description: Bot authentication token obtained from @BotFather (embedded in URL path)\n  sources:\n  - openapi/telegram-bot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/authentication/telegram-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bots
- Chat
- Messaging
- Notification
- Payments
- Telegram
---
