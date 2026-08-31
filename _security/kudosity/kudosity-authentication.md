---
api_key_in:
- header
api_specs:
- filename: kudosity-account-api-openapi.yml
  format: yaml
  label: Kudosity Account API
  slug: kudosity-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-account-api-openapi.yml
- filename: kudosity-contacts-lists-api-openapi.yml
  format: yaml
  label: Kudosity Contacts & Lists API
  slug: kudosity-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-contacts-lists-api-openapi.yml
- filename: kudosity-email-sms-api-openapi.yml
  format: yaml
  label: Kudosity Email SMS API
  slug: kudosity-email-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-email-sms-api-openapi.yml
- filename: kudosity-keywords-api-openapi.yml
  format: yaml
  label: Kudosity Keywords API
  slug: kudosity-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-keywords-api-openapi.yml
- filename: kudosity-mms-api-openapi.yml
  format: yaml
  label: Kudosity MMS API
  slug: kudosity-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-mms-api-openapi.yml
- filename: kudosity-numbers-api-openapi.yml
  format: yaml
  label: Kudosity Numbers API
  slug: kudosity-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-numbers-api-openapi.yml
- filename: kudosity-rcs-api-openapi.yml
  format: yaml
  label: Kudosity RCS API
  slug: kudosity-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-rcs-api-openapi.yml
- filename: kudosity-reporting-api-openapi.yml
  format: yaml
  label: Kudosity Reporting API
  slug: kudosity-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-reporting-api-openapi.yml
- filename: kudosity-senders-api-openapi.yml
  format: yaml
  label: Kudosity Senders API
  slug: kudosity-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-senders-api-openapi.yml
- filename: kudosity-sms-api-openapi.yml
  format: yaml
  label: Kudosity SMS API
  slug: kudosity-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-sms-api-openapi.yml
- filename: kudosity-webhook-api-openapi.yml
  format: yaml
  label: Kudosity Webhook API
  slug: kudosity-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-webhook-api-openapi.yml
- filename: kudosity-whatsapp-api-openapi.yml
  format: yaml
  label: Kudosity Whats App API
  slug: kudosity-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-whatsapp-api-openapi.yml
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
- Webhook
- MCP
- Agent-native
- Australia
- Notification
- Two-Way Messaging
- Contact Management
---
