---
api_key_in:
- header
api_specs:
- filename: telefonie-voice-openapi.yml
  format: yaml
  label: Telefonie Voice API
  slug: telefonie-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-voice-openapi.yml
- filename: telefonie-sms-openapi.yml
  format: yaml
  label: Telefonie SMS API
  slug: telefonie-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-sms-openapi.yml
- filename: telefonie-numbers-openapi.yml
  format: yaml
  label: Telefonie Number Management API
  slug: telefonie-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-numbers-openapi.yml
- filename: telefonie-recording-openapi.yml
  format: yaml
  label: Telefonie Call Recording API
  slug: telefonie-call-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonie/refs/heads/main/openapi/telefonie-recording-openapi.yml
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
