---
api_key_in:
- header
api_specs:
- filename: telefon-available-numbers-api-openapi.yml
  format: yaml
  label: Telefon Available Numbers API
  slug: telefon-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-available-numbers-api-openapi.yml
- filename: telefon-calls-api-openapi.yml
  format: yaml
  label: Telefon Calls API
  slug: telefon-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-calls-api-openapi.yml
- filename: telefon-conferences-api-openapi.yml
  format: yaml
  label: Telefon Conferences API
  slug: telefon-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-conferences-api-openapi.yml
- filename: telefon-messages-api-openapi.yml
  format: yaml
  label: Telefon Messages API
  slug: telefon-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-messages-api-openapi.yml
- filename: telefon-owned-numbers-api-openapi.yml
  format: yaml
  label: Telefon Owned Numbers API
  slug: telefon-owned-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-owned-numbers-api-openapi.yml
- filename: telefon-recordings-api-openapi.yml
  format: yaml
  label: Telefon Recordings API
  slug: telefon-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-recordings-api-openapi.yml
- filename: telefon-transcriptions-api-openapi.yml
  format: yaml
  label: Telefon Transcriptions API
  slug: telefon-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-transcriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Telefon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telefon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telefon
provider_slug: telefon
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/telefon-numbers-openapi.yml
  - openapi/telefon-recording-openapi.yml
  - openapi/telefon-sms-openapi.yml
  - openapi/telefon-voice-openapi.yml
  type: apiKey
slug: telefon-authentication
source_filename: telefon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telefon-numbers-openapi.yml, openapi/telefon-recording-openapi.yml, openapi/telefon-sms-openapi.yml,\n  openapi/telefon-voice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/telefon-numbers-openapi.yml\n  - openapi/telefon-recording-openapi.yml\n  - openapi/telefon-sms-openapi.yml\n  - openapi/telefon-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/authentication/telefon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Call Recording
- Communications
- CPaaS
- Global Coverage
- Messaging
- Number Provisioning
- SMS
- Telephony
- Voice
- VoIP
---
