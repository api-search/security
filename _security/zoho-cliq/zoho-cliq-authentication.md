---
api_key_in: []
api_specs:
- filename: chats.yml
  format: yaml
  label: Zoho Cliq API
  slug: zoho-cliq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-cliq/refs/heads/main/openapi/chats.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Cliq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Zoho Cliq secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Zoho Cliq
provider_slug: zoho-cliq
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
    scopes: 7
  name: Cliq_Auth
  sources:
  - openapi/bots.yml
  - openapi/buttons.yml
  - openapi/chats.yml
  - openapi/datastores.yml
  - openapi/dndsettings.yml
  - openapi/extensions.yml
  - openapi/functions.yml
  - openapi/keyboardshortcuts.yml
  - openapi/mentions.yml
  - openapi/messageactions.yml
  - openapi/messagecards.yml
  - openapi/messageformat.yml
  - openapi/messages.yml
  - openapi/mobilesettings.yml
  - openapi/mypins.yml
  - openapi/pinmessages.yml
  - openapi/reminders.yml
  - openapi/scheduledmessages.yml
  - openapi/slashcommands.yml
  - openapi/threads.yml
  - openapi/userpreferences.yml
  type: oauth2
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: Cliq_Auth
  sources:
  - openapi/stars.yml
  type: oauth2
slug: zoho-cliq-authentication
source_filename: zoho-cliq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bots.yml, openapi/buttons.yml, openapi/chats.yml, openapi/datastores.yml, openapi/dndsettings.yml,\n  openapi/extensions.yml, openapi/functions.yml, openapi/keyboardshortcuts.yml, openapi/mentions.yml,\n  openapi/messageactions.yml, openapi/messagecards.yml, openapi/messageformat.yml ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: Cliq_Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    scopes: 7\n  sources:\n  - openapi/bots.yml\n  - openapi/buttons.yml\n  - openapi/chats.yml\n  - openapi/datastores.yml\n  - openapi/dndsettings.yml\n  - openapi/extensions.yml\n  - openapi/functions.yml\n  - openapi/keyboardshortcuts.yml\n  - openapi/mentions.yml\n  - openapi/messageactions.yml\n  - openapi/messagecards.yml\n  - openapi/messageformat.yml\n  - openapi/messages.yml\n  - openapi/mobilesettings.yml\n\
  \  - openapi/mypins.yml\n  - openapi/pinmessages.yml\n  - openapi/reminders.yml\n  - openapi/scheduledmessages.yml\n  - openapi/slashcommands.yml\n  - openapi/threads.yml\n  - openapi/userpreferences.yml\n- name: Cliq_Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 4\n  sources:\n  - openapi/stars.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-cliq/refs/heads/main/authentication/zoho-cliq-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Messaging
- Team Collaboration
- Chat
- Bots
- Webhooks
- Slash Commands
- Communication
---
