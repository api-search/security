---
api_key_in: []
api_specs:
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Tickets API
  slug: trengo-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Contacts API
  slug: trengo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Messages API
  slug: trengo-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Channels API
  slug: trengo-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Teams and Users API
  slug: trengo-teams-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Labels and Custom Fields API
  slug: trengo-labels-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Webhooks API
  slug: trengo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo WhatsApp Templates API
  slug: trengo-whatsapp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trengo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trengo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trengo
provider_slug: trengo
scheme_count: 1
schemes:
- description: 'Personal access token generated in the Trengo account, sent as `Authorization: Bearer {TOKEN}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trengo-openapi.yml
  type: http
slug: trengo-authentication
source_filename: trengo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trengo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token generated in the Trengo account, sent as `Authorization:\n    Bearer {TOKEN}`.'\n  sources:\n  - openapi/trengo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/authentication/trengo-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Engagement
- Omnichannel
- Shared Inbox
- Messaging
- WhatsApp
- Customer Support
---
