---
api_key_in:
- path
api_specs:
- filename: telegram-bot-openapi.yml
  format: yaml
  label: Telegram Bot API
  slug: telegram-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-bot-openapi.yml
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
- Notifications
- Payments
- Telegram
---
