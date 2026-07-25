---
api_key_in: []
api_specs:
- filename: clicksend-account-api-openapi.yml
  format: yaml
  label: ClickSend Account API
  slug: clicksend-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-account-api-openapi.yml
- filename: clicksend-contact-api-openapi.yml
  format: yaml
  label: ClickSend Contact API
  slug: clicksend-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-contact-api-openapi.yml
- filename: clicksend-contactlist-api-openapi.yml
  format: yaml
  label: ClickSend ContactList API
  slug: clicksend-contactlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-contactlist-api-openapi.yml
- filename: clicksend-email-api-openapi.yml
  format: yaml
  label: ClickSend Email API
  slug: clicksend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-email-api-openapi.yml
- filename: clicksend-mms-api-openapi.yml
  format: yaml
  label: ClickSend MMS API
  slug: clicksend-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-mms-api-openapi.yml
- filename: clicksend-post-letter-api-openapi.yml
  format: yaml
  label: ClickSend Post Letter API
  slug: clicksend-post-letter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-post-letter-api-openapi.yml
- filename: clicksend-post-postcard-api-openapi.yml
  format: yaml
  label: ClickSend Post Postcard API
  slug: clicksend-post-postcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-post-postcard-api-openapi.yml
- filename: clicksend-receipts-api-openapi.yml
  format: yaml
  label: ClickSend Receipts API
  slug: clicksend-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-receipts-api-openapi.yml
- filename: clicksend-sms-api-openapi.yml
  format: yaml
  label: ClickSend SMS API
  slug: clicksend-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-sms-api-openapi.yml
- filename: clicksend-voice-api-openapi.yml
  format: yaml
  label: ClickSend Voice API
  slug: clicksend-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-voice-api-openapi.yml
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
