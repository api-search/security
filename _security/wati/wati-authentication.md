---
api_key_in: []
api_specs:
- filename: wati-openapi.yml
  format: yaml
  label: WATI WhatsApp Business API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/openapi/wati-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wati Authentication
name_suffix: Authentication
oauth_flows: []
overview: WATI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WATI
provider_slug: wati
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'WATI uses Bearer token authentication. Tokens are issued from the WATI

    dashboard under API Docs and must be supplied as

    `Authorization: Bearer <token>` on every request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wati-openapi.yml
  type: http
slug: wati-authentication
source_filename: wati-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wati-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    WATI uses Bearer token authentication. Tokens are issued from the WATI\n    dashboard under API Docs and must be supplied as\n    `Authorization: Bearer <token>` on every request.\n  sources:\n  - openapi/wati-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/authentication/wati-authentication.yml
summary_line: http · 1 scheme
tags:
- WhatsApp
- Messaging
- Customer Engagement
- Chatbot
- Business Communication
- CRM
---
