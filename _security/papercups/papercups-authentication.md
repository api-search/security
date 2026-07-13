---
api_key_in: []
api_specs:
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-openapi.yml
  format: yaml
  label: Papercups Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/openapi/papercups-openapi.yml
- filename: papercups-asyncapi.yml
  format: yaml
  label: Papercups Realtime Chat API (WebSocket / Phoenix Channels)
  slug: realtime-chat
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/asyncapi/papercups-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Papercups Authentication
name_suffix: Authentication
oauth_flows: []
overview: Papercups secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Papercups
provider_slug: papercups
scheme_count: 1
schemes:
- description: 'Bearer API key (personal API key / token) from the Papercups dashboard, sent as `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/papercups-openapi.yml
  type: http
slug: papercups-authentication
source_filename: papercups-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/papercups-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key (personal API key / token) from the Papercups dashboard, sent\n    as `Authorization: Bearer <API_KEY>`.'\n  sources:\n  - openapi/papercups-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papercups/refs/heads/main/authentication/papercups-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Messaging
- Live Chat
- Open Source
- Support
- Intercom Alternative
---
