---
api_key_in:
- header
api_specs:
- filename: brevo-transactional-email-openapi.yml
  format: yaml
  label: Brevo Transactional Email API
  slug: transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-transactional-email-openapi.yml
- filename: brevo-email-campaigns-openapi.yml
  format: yaml
  label: Brevo Email Campaigns API
  slug: email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-email-campaigns-openapi.yml
- filename: brevo-contacts-openapi.yml
  format: yaml
  label: Brevo Contacts API
  slug: contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-contacts-openapi.yml
- filename: brevo-transactional-sms-openapi.yml
  format: yaml
  label: Brevo Transactional SMS API
  slug: transactional-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-transactional-sms-openapi.yml
- filename: brevo-whatsapp-openapi.yml
  format: yaml
  label: Brevo WhatsApp API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-whatsapp-openapi.yml
- filename: brevo-ecommerce-openapi.yml
  format: yaml
  label: Brevo eCommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-ecommerce-openapi.yml
- filename: brevo-conversations-openapi.yml
  format: yaml
  label: Brevo Conversations API
  slug: conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-conversations-openapi.yml
- filename: brevo-webhooks-openapi.yml
  format: yaml
  label: Brevo Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-webhooks-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brevo Authentication
name_suffix: Authentication
oauth_flows: []
overview: brevo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: brevo
provider_slug: brevo
scheme_count: 1
schemes:
- description: Brevo API key passed in the api-key request header for authentication.
  in: header
  name: apiKeyAuth
  parameter: api-key
  sources:
  - openapi/brevo-contacts-openapi.yml
  - openapi/brevo-conversations-openapi.yml
  - openapi/brevo-ecommerce-openapi.yml
  - openapi/brevo-email-campaigns-openapi.yml
  - openapi/brevo-transactional-email-openapi.yml
  - openapi/brevo-transactional-sms-openapi.yml
  - openapi/brevo-webhooks-openapi.yml
  - openapi/brevo-whatsapp-openapi.yml
  type: apiKey
slug: brevo-authentication
source_filename: brevo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brevo-contacts-openapi.yml, openapi/brevo-conversations-openapi.yml, openapi/brevo-ecommerce-openapi.yml,\n  openapi/brevo-email-campaigns-openapi.yml, openapi/brevo-transactional-email-openapi.yml,\n  openapi/brevo-transactional-sms-openapi.yml, openapi/brevo-webhooks-openapi.yml, openapi/brevo-whatsapp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Brevo API key passed in the api-key request header for authentication.\n  sources:\n  - openapi/brevo-contacts-openapi.yml\n  - openapi/brevo-conversations-openapi.yml\n  - openapi/brevo-ecommerce-openapi.yml\n  - openapi/brevo-email-campaigns-openapi.yml\n  - openapi/brevo-transactional-email-openapi.yml\n  - openapi/brevo-transactional-sms-openapi.yml\n  - openapi/brevo-webhooks-openapi.yml\n  - openapi/brevo-whatsapp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/authentication/brevo-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
