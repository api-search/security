---
api_key_in:
- header
api_specs:
- filename: kudosity-transmit-message-openapi-original.yml
  format: yaml
  label: Transmit Message API
  slug: transmit-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-transmit-message-openapi-original.yml
- filename: kudosity-transmit-sms-openapi-original.yml
  format: yaml
  label: Transmit SMS API
  slug: transmit-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-transmit-sms-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kudosity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kudosity secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kudosity
provider_slug: kudosity
scheme_count: 2
schemes:
- description: All API requests require your API credentials, you will find them once logged into your account on the SETTINGS page. Scroll down to API Settings to find your API key.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/kudosity-transmit-message-openapi-original.yml
  type: apiKey
- description: 'Use the `Authorization` header with the value `Basic {base64(api_key:api_secret)}`.

    - `api_key`: Your API key

    - `api_secret`: Your API secret'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kudosity-transmit-sms-openapi-original.yml
  type: http
slug: kudosity-authentication
source_filename: kudosity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/kudosity-transmit-message-openapi-original.yml, openapi/kudosity-transmit-sms-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: All API requests require your API credentials, you will find them once logged\n    into your account on the SETTINGS page. Scroll down to API Settings to find your API key.\n  sources:\n  - openapi/kudosity-transmit-message-openapi-original.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Use the `Authorization` header with the value `Basic {base64(api_key:api_secret)}`.\n    - `api_key`: Your API key\n    - `api_secret`: Your API secret\n  sources:\n  - openapi/kudosity-transmit-sms-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/authentication/kudosity-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Messaging
- SMS
- MMS
- RCS
- WhatsApp
- Communications
- CPaaS
- Webhooks
- MCP
- Agent-native
- Australia
- Notifications
- Two-Way Messaging
- Contact Management
---
