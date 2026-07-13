---
api_key_in: []
api_specs:
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Messaging API
  slug: gupshup-whatsapp-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Template Messaging API
  slug: gupshup-whatsapp-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Opt-In Management API
  slug: gupshup-whatsapp-optin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gupshup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gupshup secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gupshup
provider_slug: gupshup
scheme_count: 1
schemes:
- description: 'Account API key sent in the `apikey` HTTP request header on every call to api.gupshup.io. Obtained from the Gupshup dashboard. The key scopes requests to your account; individual operations additionally reference a registered app by name (`src.name` field or the appName path segment). Self-serve - no OAuth flow. The Partner API (partner.gupshup.io) uses a different model: a partner token / app access token passed in the Authorization header rather than the per-app apikey.'
  in: header
  keyName: apikey
  name: apiKeyAuth
  sources:
  - openapi/gupshup-openapi.yml
  - https://docs.gupshup.io/reference/msg
  type: apiKey
slug: gupshup-authentication
source_filename: gupshup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/gupshup-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: apikey\n  description: >-\n    Account API key sent in the `apikey` HTTP request header on every call to\n    api.gupshup.io. Obtained from the Gupshup dashboard. The key scopes requests\n    to your account; individual operations additionally reference a registered app\n    by name (`src.name` field or the appName path segment). Self-serve - no OAuth\n    flow. The Partner API (partner.gupshup.io) uses a different model: a partner\n    token / app access token passed in the Authorization header rather than the\n    per-app apikey.\n  sources:\n  - openapi/gupshup-openapi.yml\n  - https://docs.gupshup.io/reference/msg\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/authentication/gupshup-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Messaging
- WhatsApp
- Conversational AI
- CPaaS
- SMS
- RCS
- India
- Chatbots
- Business Messaging
- Communications
---
