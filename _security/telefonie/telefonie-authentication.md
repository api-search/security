---
api_key_in:
- header
api_specs:
- filename: telefonie-available-numbers-api-openapi.yml
  format: yaml
  label: Telefonie Available Numbers API
  slug: telefonie-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-available-numbers-api-openapi.yml
- filename: telefonie-calls-api-openapi.yml
  format: yaml
  label: Telefonie Calls API
  slug: telefonie-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-calls-api-openapi.yml
- filename: telefonie-conferences-api-openapi.yml
  format: yaml
  label: Telefonie Conferences API
  slug: telefonie-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-conferences-api-openapi.yml
- filename: telefonie-messages-api-openapi.yml
  format: yaml
  label: Telefonie Messages API
  slug: telefonie-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-messages-api-openapi.yml
- filename: telefonie-owned-numbers-api-openapi.yml
  format: yaml
  label: Telefonie Owned Numbers API
  slug: telefonie-owned-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-owned-numbers-api-openapi.yml
- filename: telefonie-recordings-api-openapi.yml
  format: yaml
  label: Telefonie Recordings API
  slug: telefonie-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-recordings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Telefonie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telefonie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telefonie
provider_slug: telefonie
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/telefonie-numbers-openapi.yml
  - openapi/telefonie-recording-openapi.yml
  - openapi/telefonie-sms-openapi.yml
  - openapi/telefonie-voice-openapi.yml
  type: apiKey
slug: telefonie-authentication
source_filename: telefonie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telefonie-numbers-openapi.yml, openapi/telefonie-recording-openapi.yml, openapi/telefonie-sms-openapi.yml,\n  openapi/telefonie-voice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/telefonie-numbers-openapi.yml\n  - openapi/telefonie-recording-openapi.yml\n  - openapi/telefonie-sms-openapi.yml\n  - openapi/telefonie-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/authentication/telefonie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Call Recording
- CPaaS
- Messaging
- Number Provisioning
- SMS
- Telecommunications
- Telephony
- Voice
- VoIP
---
