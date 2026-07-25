---
api_key_in: []
api_specs:
- filename: clicksend-sms-sms-api-openapi.yml
  format: yaml
  label: ClickSend SMS Sms API
  slug: clicksend-sms-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend-sms/refs/heads/main/openapi/clicksend-sms-sms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clicksend Sms Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickSend SMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClickSend SMS
provider_slug: clicksend-sms
scheme_count: 1
schemes:
- description: Username and API key
  name: basicAuth
  scheme: basic
  sources:
  - openapi/clicksend-sms-openapi.yml
  type: http
slug: clicksend-sms-authentication
source_filename: clicksend-sms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clicksend-sms-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username and API key\n  sources:\n  - openapi/clicksend-sms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicksend-sms/refs/heads/main/authentication/clicksend-sms-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- MMS
- Messaging
- Voice
- Email
- Fax
- Direct Mail
- Communications
---
