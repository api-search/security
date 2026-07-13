---
api_key_in: []
api_specs:
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Comments API
  slug: comments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Tags and Custom Fields API
  slug: tags-custom-fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
- filename: respond-openapi.yml
  format: yaml
  label: Respond.io Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Respond Authentication
name_suffix: Authentication
oauth_flows: []
overview: Respond.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Respond.io
provider_slug: respond
scheme_count: 1
schemes:
- description: API Access Token from Settings > Integrations > Developer API, sent in the Authorization header as `Bearer {token}`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/respond-openapi.yml
  type: http
slug: respond-authentication
source_filename: respond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/respond-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API Access Token from Settings > Integrations > Developer API, sent in the Authorization\n    header as `Bearer {token}`.\n  sources:\n  - openapi/respond-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/authentication/respond-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- Omnichannel
- Customer Conversations
- WhatsApp
- AI
---
