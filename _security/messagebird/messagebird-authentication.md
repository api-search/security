---
api_key_in:
- header
api_specs:
- filename: messagebird-sms-messaging-openapi.yml
  format: yaml
  label: MessageBird SMS Messaging API
  slug: sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-sms-messaging-openapi.yml
- filename: messagebird-voice-calling-openapi.yml
  format: yaml
  label: MessageBird Voice Calling API
  slug: voice-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-calling-openapi.yml
- filename: messagebird-voice-messaging-openapi.yml
  format: yaml
  label: MessageBird Voice Messaging API
  slug: voice-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messaging-openapi.yml
- filename: messagebird-conversations-openapi.yml
  format: yaml
  label: MessageBird Conversations API
  slug: conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-openapi.yml
- filename: messagebird-whatsapp-openapi.yml
  format: yaml
  label: MessageBird WhatsApp API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-whatsapp-openapi.yml
- filename: messagebird-verify-openapi.yml
  format: yaml
  label: MessageBird Verify API
  slug: verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-openapi.yml
- filename: messagebird-lookup-openapi.yml
  format: yaml
  label: MessageBird Lookup API
  slug: lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-openapi.yml
- filename: messagebird-hlr-openapi.yml
  format: yaml
  label: MessageBird HLR API
  slug: hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-openapi.yml
- filename: messagebird-contacts-openapi.yml
  format: yaml
  label: MessageBird Contacts API
  slug: contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-openapi.yml
- filename: messagebird-numbers-openapi.yml
  format: yaml
  label: MessageBird Numbers API
  slug: numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-numbers-openapi.yml
- filename: messagebird-balance-openapi.yml
  format: yaml
  label: MessageBird Balance API
  slug: balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-openapi.yml
- filename: messagebird-integrations-openapi.yml
  format: yaml
  label: MessageBird Integrations API
  slug: integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-integrations-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Messagebird Authentication
name_suffix: Authentication
oauth_flows: []
overview: messagebird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: messagebird
provider_slug: messagebird
scheme_count: 1
schemes:
- description: Access key authentication in the form of 'AccessKey {accessKey}'.
  in: header
  name: accessKey
  parameter: Authorization
  sources:
  - openapi/messagebird-balance-openapi.yml
  - openapi/messagebird-contacts-openapi.yml
  - openapi/messagebird-conversations-openapi.yml
  - openapi/messagebird-hlr-openapi.yml
  - openapi/messagebird-integrations-openapi.yml
  - openapi/messagebird-lookup-openapi.yml
  - openapi/messagebird-numbers-openapi.yml
  - openapi/messagebird-sms-messaging-openapi.yml
  - openapi/messagebird-verify-openapi.yml
  - openapi/messagebird-voice-calling-openapi.yml
  - openapi/messagebird-voice-messaging-openapi.yml
  - openapi/messagebird-whatsapp-openapi.yml
  type: apiKey
slug: messagebird-authentication
source_filename: messagebird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/messagebird-balance-openapi.yml, openapi/messagebird-contacts-openapi.yml, openapi/messagebird-conversations-openapi.yml,\n  openapi/messagebird-hlr-openapi.yml, openapi/messagebird-integrations-openapi.yml, openapi/messagebird-lookup-openapi.yml,\n  openapi/messagebird-numbers-openapi.yml, openapi/messagebird-sms-messaging-openapi.yml, openapi/messagebird-verify-openapi.yml,\n  openapi/messagebird-voice-calling-openapi.yml, openapi/messagebird-voice-messaging-openapi.yml,\n  openapi/messagebird-whatsapp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Access key authentication in the form of 'AccessKey {accessKey}'.\n  sources:\n  - openapi/messagebird-balance-openapi.yml\n  - openapi/messagebird-contacts-openapi.yml\n  - openapi/messagebird-conversations-openapi.yml\n  - openapi/messagebird-hlr-openapi.yml\n\
  \  - openapi/messagebird-integrations-openapi.yml\n  - openapi/messagebird-lookup-openapi.yml\n  - openapi/messagebird-numbers-openapi.yml\n  - openapi/messagebird-sms-messaging-openapi.yml\n  - openapi/messagebird-verify-openapi.yml\n  - openapi/messagebird-voice-calling-openapi.yml\n  - openapi/messagebird-voice-messaging-openapi.yml\n  - openapi/messagebird-whatsapp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/authentication/messagebird-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
