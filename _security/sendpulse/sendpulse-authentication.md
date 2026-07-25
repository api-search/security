---
api_key_in: []
api_specs:
- filename: sendpulse-account-api-openapi.yml
  format: yaml
  label: SendPulse Account API
  slug: sendpulse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-account-api-openapi.yml
- filename: sendpulse-address-books-api-openapi.yml
  format: yaml
  label: SendPulse Address Books API
  slug: sendpulse-address-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-address-books-api-openapi.yml
- filename: sendpulse-authorization-api-openapi.yml
  format: yaml
  label: SendPulse Authorization API
  slug: sendpulse-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-authorization-api-openapi.yml
- filename: sendpulse-automation-360-api-openapi.yml
  format: yaml
  label: SendPulse Automation 360 API
  slug: sendpulse-automation-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-automation-360-api-openapi.yml
- filename: sendpulse-email-blacklist-api-openapi.yml
  format: yaml
  label: SendPulse Email Blacklist API
  slug: sendpulse-email-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-email-blacklist-api-openapi.yml
- filename: sendpulse-email-campaigns-api-openapi.yml
  format: yaml
  label: SendPulse Email Campaigns API
  slug: sendpulse-email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-email-campaigns-api-openapi.yml
- filename: sendpulse-senders-api-openapi.yml
  format: yaml
  label: SendPulse Senders API
  slug: sendpulse-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-senders-api-openapi.yml
- filename: sendpulse-sms-api-openapi.yml
  format: yaml
  label: SendPulse SMS API
  slug: sendpulse-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-sms-api-openapi.yml
- filename: sendpulse-smtp-api-openapi.yml
  format: yaml
  label: SendPulse SMTP API
  slug: sendpulse-smtp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-smtp-api-openapi.yml
- filename: sendpulse-web-push-api-openapi.yml
  format: yaml
  label: SendPulse Web Push API
  slug: sendpulse-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-web-push-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sendpulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: SendPulse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SendPulse
provider_slug: sendpulse
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token obtained from POST /oauth/access_token using the client_credentials grant.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sendpulse-openapi.yml
  type: http
slug: sendpulse-authentication
source_filename: sendpulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendpulse-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token obtained from POST /oauth/access_token using the client_credentials\n    grant.\n  sources:\n  - openapi/sendpulse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/authentication/sendpulse-authentication.yml
summary_line: http · 1 scheme
tags:
- Marketing
- Email
- SMS
- Web Push
- Chatbots
- Transactional Email
- Multichannel
---
