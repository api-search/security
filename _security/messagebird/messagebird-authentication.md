---
api_key_in:
- header
api_specs:
- filename: messagebird-available-numbers-api-openapi.yml
  format: yaml
  label: messagebird Available Numbers API
  slug: messagebird-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-available-numbers-api-openapi.yml
- filename: messagebird-balance-api-openapi.yml
  format: yaml
  label: messagebird Balance API
  slug: messagebird-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-api-openapi.yml
- filename: messagebird-call-flows-api-openapi.yml
  format: yaml
  label: messagebird Call Flows API
  slug: messagebird-call-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-call-flows-api-openapi.yml
- filename: messagebird-calls-api-openapi.yml
  format: yaml
  label: messagebird Calls API
  slug: messagebird-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-calls-api-openapi.yml
- filename: messagebird-contacts-api-openapi.yml
  format: yaml
  label: messagebird Contacts API
  slug: messagebird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-api-openapi.yml
- filename: messagebird-conversations-api-openapi.yml
  format: yaml
  label: messagebird Conversations API
  slug: messagebird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-api-openapi.yml
- filename: messagebird-groups-api-openapi.yml
  format: yaml
  label: messagebird Groups API
  slug: messagebird-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-groups-api-openapi.yml
- filename: messagebird-hlr-api-openapi.yml
  format: yaml
  label: messagebird HLR API
  slug: messagebird-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-api-openapi.yml
- filename: messagebird-legs-api-openapi.yml
  format: yaml
  label: messagebird Legs API
  slug: messagebird-legs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-legs-api-openapi.yml
- filename: messagebird-lookup-api-openapi.yml
  format: yaml
  label: messagebird Lookup API
  slug: messagebird-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-api-openapi.yml
- filename: messagebird-messages-api-openapi.yml
  format: yaml
  label: messagebird Messages API
  slug: messagebird-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-messages-api-openapi.yml
- filename: messagebird-purchased-numbers-api-openapi.yml
  format: yaml
  label: messagebird Purchased Numbers API
  slug: messagebird-purchased-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-purchased-numbers-api-openapi.yml
- filename: messagebird-recordings-api-openapi.yml
  format: yaml
  label: messagebird Recordings API
  slug: messagebird-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-recordings-api-openapi.yml
- filename: messagebird-templates-api-openapi.yml
  format: yaml
  label: messagebird Templates API
  slug: messagebird-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-templates-api-openapi.yml
- filename: messagebird-transcriptions-api-openapi.yml
  format: yaml
  label: messagebird Transcriptions API
  slug: messagebird-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-transcriptions-api-openapi.yml
- filename: messagebird-verify-api-openapi.yml
  format: yaml
  label: messagebird Verify API
  slug: messagebird-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-api-openapi.yml
- filename: messagebird-voice-messages-api-openapi.yml
  format: yaml
  label: messagebird Voice Messages API
  slug: messagebird-voice-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messages-api-openapi.yml
- filename: messagebird-webhooks-api-openapi.yml
  format: yaml
  label: messagebird Webhooks API
  slug: messagebird-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-webhooks-api-openapi.yml
- filename: messagebird-whatsapp-messages-api-openapi.yml
  format: yaml
  label: messagebird WhatsApp Messages API
  slug: messagebird-whatsapp-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-whatsapp-messages-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Messagebird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messagebird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Messagebird
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
