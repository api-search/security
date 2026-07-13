---
api_key_in: []
api_specs:
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend SMS API
  slug: clicksend-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend MMS API
  slug: clicksend-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Voice / Text-to-Speech API
  slug: clicksend-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Transactional Email API
  slug: clicksend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Letters API
  slug: clicksend-post-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Postcards API
  slug: clicksend-post-postcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Contacts & Lists API
  slug: clicksend-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Delivery Receipts & Inbound API
  slug: clicksend-delivery-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Account & Balance API
  slug: clicksend-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clicksend Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickSend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClickSend
provider_slug: clicksend
scheme_count: 1
schemes:
- description: HTTP Basic authentication using your ClickSend username and API key. The username is your ClickSend account username; the password is your API key from the ClickSend dashboard.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/clicksend-openapi.yml
  type: http
slug: clicksend-authentication
source_filename: clicksend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clicksend-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your ClickSend username and API key. The username\n    is your ClickSend account username; the password is your API key from the ClickSend dashboard.\n  sources:\n  - openapi/clicksend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/authentication/clicksend-authentication.yml
summary_line: http · 1 scheme
tags:
- Communications
- SMS
- MMS
- Voice
- Email
- Post
- Messaging
- CPaaS
---
