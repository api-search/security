---
api_key_in: []
api_specs:
- filename: manychat-openapi.yml
  format: yaml
  label: ManyChat REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Manychat Authentication
name_suffix: Authentication
oauth_flows: []
overview: ManyChat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ManyChat
provider_slug: manychat
scheme_count: 1
schemes:
- description: Bearer token of the form `Bearer <page-id>:<api-key>` issued from the ManyChat dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/manychat-openapi.yml
  type: http
slug: manychat-authentication
source_filename: manychat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/manychat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token of the form `Bearer <page-id>:<api-key>` issued from the ManyChat\n    dashboard.\n  sources:\n  - openapi/manychat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/authentication/manychat-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat Marketing
- Messenger Marketing
- Conversational Commerce
- Marketing Automation
- Instagram
- WhatsApp
- Facebook Messenger
---
