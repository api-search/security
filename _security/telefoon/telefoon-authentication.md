---
api_key_in:
- header
api_specs:
- filename: telefoon-voice-openapi.yml
  format: yaml
  label: Telefoon Voice API
  slug: telefoon-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-voice-openapi.yml
- filename: telefoon-sms-openapi.yml
  format: yaml
  label: Telefoon SMS API
  slug: telefoon-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-sms-openapi.yml
- filename: telefoon-numbers-openapi.yml
  format: yaml
  label: Telefoon Number Management API
  slug: telefoon-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-numbers-openapi.yml
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
