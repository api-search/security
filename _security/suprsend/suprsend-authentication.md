---
api_key_in:
- header
api_specs:
- filename: suprsend-rest-api-openapi.yml
  format: yaml
  label: SuprSend REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suprsend/refs/heads/main/openapi/suprsend-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Suprsend Authentication
name_suffix: Authentication
oauth_flows: []
overview: SuprSend secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SuprSend
provider_slug: suprsend
scheme_count: 3
schemes:
- bearerFormat: API_Key
  description: Pass as `Bearer <API_KEY>`. Get API Key from SuprSend dashboard Developers -> API Keys section.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/suprsend-rest-api-openapi.yml
  type: http
- description: You can get Service Token from [SuprSend dashboard -> Account Settings -> Service Tokens](https://app.suprsend.com/en/account-settings/service-tokens) section.
  in: header
  name: ServiceTokenAuth
  parameter: ServiceToken <token>
  sources:
  - openapi/suprsend-rest-api-openapi.yml
  type: apiKey
- description: Bearer authentication header of the form `Bearer <token>`, where <token> is your auth token.
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/suprsend-rest-api-openapi.yml
  type: apiKey
slug: suprsend-authentication
source_filename: suprsend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suprsend-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_Key\n  description: Pass as `Bearer <API_KEY>`. Get API Key from SuprSend dashboard Developers ->\n    API Keys section.\n  sources:\n  - openapi/suprsend-rest-api-openapi.yml\n- name: ServiceTokenAuth\n  type: apiKey\n  in: header\n  parameter: ServiceToken <token>\n  description: You can get Service Token from [SuprSend dashboard -> Account Settings -> Service\n    Tokens](https://app.suprsend.com/en/account-settings/service-tokens) section.\n  sources:\n  - openapi/suprsend-rest-api-openapi.yml\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer authentication header of the form `Bearer <token>`, where <token> is your\n    auth token.\n  sources:\n  - openapi/suprsend-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suprsend/refs/heads/main/authentication/suprsend-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Notifications
- Multi-Channel
- Email
- SMS
- Push Notifications
- In-App Inbox
- WhatsApp
- Slack
- Notification Infrastructure
- Workflow Automation
- Template Management
---
