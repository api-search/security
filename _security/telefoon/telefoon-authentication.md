---
api_key_in:
- header
api_specs:
- filename: telefoon-available-numbers-api-openapi.yml
  format: yaml
  label: Telefoon Available Numbers API
  slug: telefoon-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-available-numbers-api-openapi.yml
- filename: telefoon-calls-api-openapi.yml
  format: yaml
  label: Telefoon Calls API
  slug: telefoon-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-calls-api-openapi.yml
- filename: telefoon-conferences-api-openapi.yml
  format: yaml
  label: Telefoon Conferences API
  slug: telefoon-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-conferences-api-openapi.yml
- filename: telefoon-messages-api-openapi.yml
  format: yaml
  label: Telefoon Messages API
  slug: telefoon-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-messages-api-openapi.yml
- filename: telefoon-owned-numbers-api-openapi.yml
  format: yaml
  label: Telefoon Owned Numbers API
  slug: telefoon-owned-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-owned-numbers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Telefoon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telefoon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telefoon
provider_slug: telefoon
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/telefoon-numbers-openapi.yml
  - openapi/telefoon-sms-openapi.yml
  - openapi/telefoon-voice-openapi.yml
  type: apiKey
slug: telefoon-authentication
source_filename: telefoon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telefoon-numbers-openapi.yml, openapi/telefoon-sms-openapi.yml, openapi/telefoon-voice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/telefoon-numbers-openapi.yml\n  - openapi/telefoon-sms-openapi.yml\n  - openapi/telefoon-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/authentication/telefoon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Belgium
- CPaaS
- EU Data Residency
- Europe
- GDPR Compliant
- Messaging
- Netherlands
- Number Provisioning
- SMS
- Telephony
- Voice
---
