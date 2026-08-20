---
api_key_in: []
api_specs:
- filename: respond-comments-api-openapi.yml
  format: yaml
  label: Respond.io Comments API
  slug: respond-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-comments-api-openapi.yml
- filename: respond-contacts-api-openapi.yml
  format: yaml
  label: Respond.io Contacts API
  slug: respond-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-contacts-api-openapi.yml
- filename: respond-conversations-api-openapi.yml
  format: yaml
  label: Respond.io Conversations API
  slug: respond-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-conversations-api-openapi.yml
- filename: respond-custom-fields-api-openapi.yml
  format: yaml
  label: Respond.io Custom Fields API
  slug: respond-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-custom-fields-api-openapi.yml
- filename: respond-messages-api-openapi.yml
  format: yaml
  label: Respond.io Messages API
  slug: respond-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-messages-api-openapi.yml
- filename: respond-tags-api-openapi.yml
  format: yaml
  label: Respond.io Tags API
  slug: respond-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respond/refs/heads/main/openapi/respond-tags-api-openapi.yml
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
- Artificial Intelligence
---
