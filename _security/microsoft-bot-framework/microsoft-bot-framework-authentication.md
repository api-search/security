---
api_key_in: []
api_specs:
- filename: microsoft-bot-framework-openapi.yml
  format: yaml
  label: Bot Connector REST API
  slug: bot-connector
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bot-framework/refs/heads/main/openapi/microsoft-bot-framework-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Bot Framework Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bot Framework secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Bot Framework
provider_slug: microsoft-bot-framework
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-bot-framework-openapi.yml
  type: http
slug: microsoft-bot-framework-authentication
source_filename: microsoft-bot-framework-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bot-framework-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-bot-framework-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bot-framework/refs/heads/main/authentication/microsoft-bot-framework-authentication.yml
summary_line: http · 1 scheme
tags:
- Bots
- Conversational AI
- Messaging
- Bot Framework
- Direct Line
---
