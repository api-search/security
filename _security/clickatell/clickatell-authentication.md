---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clickatell-chat-2-pay-api-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API
  slug: clickatell-chat-2-pay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-api-openapi.yml
- filename: clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API Client Callbacks API
  slug: clickatell-chat-2-pay-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
- filename: clickatell-external-link-callback-api-openapi.yml
  format: yaml
  label: Clickatell External Link Callback API
  slug: clickatell-external-link-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-external-link-callback-api-openapi.yml
- filename: clickatell-one-api-api-openapi.yml
  format: yaml
  label: Clickatell One API
  slug: clickatell-one-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-api-openapi.yml
- filename: clickatell-one-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell One API Client Callbacks API
  slug: clickatell-one-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-client-callbacks-api-openapi.yml
- filename: clickatell-sms-api-api-openapi.yml
  format: yaml
  label: Clickatell SMS API
  slug: clickatell-sms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-api-api-openapi.yml
- filename: clickatell-sms-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell SMS Client Callbacks API
  slug: clickatell-sms-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-client-callbacks-api-openapi.yml
- filename: clickatell-wait-for-callback-api-openapi.yml
  format: yaml
  label: Clickatell Wait for Callback API
  slug: clickatell-wait-for-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-wait-for-callback-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Clickatell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clickatell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clickatell
provider_slug: clickatell
scheme_count: 1
schemes:
- description: Chat 2 Pay API Key Authorization
  in: header
  name: c2p
  parameter: Authorization
  sources:
  - openapi/clickatell-chat-2-pay-api-openapi.json
  - openapi/clickatell-one-api-openapi.json
  - openapi/clickatell-sms-api-openapi.json
  type: apiKey
slug: clickatell-authentication
source_filename: clickatell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/clickatell-chat-2-pay-api-openapi.json, openapi/clickatell-one-api-openapi.json,\n  openapi/clickatell-sms-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: c2p\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Chat 2 Pay API Key Authorization\n  sources:\n  - openapi/clickatell-chat-2-pay-api-openapi.json\n  - openapi/clickatell-one-api-openapi.json\n  - openapi/clickatell-sms-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/authentication/clickatell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- SMS
- WhatsApp
- Messaging
- CPaaS
- Chat Commerce
- Payments
---
