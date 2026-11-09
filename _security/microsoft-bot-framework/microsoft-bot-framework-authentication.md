---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-bot-framework-activities-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Activities API
  slug: microsoft-bot-framework-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-activities-api-openapi.yml
- filename: microsoft-bot-framework-attachments-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Attachments API
  slug: microsoft-bot-framework-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-attachments-api-openapi.yml
- filename: microsoft-bot-framework-conversations-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Conversations API
  slug: microsoft-bot-framework-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-conversations-api-openapi.yml
- filename: microsoft-bot-framework-members-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Members API
  slug: microsoft-bot-framework-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-members-api-openapi.yml
- filename: microsoft-bot-framework-botsignin-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Sign In API
  slug: microsoft-bot-framework-botsignin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-botsignin-api-openapi.yml
- filename: microsoft-bot-framework-user-token-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework User Token API
  slug: microsoft-bot-framework-user-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-user-token-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Microsoft Bot Framework Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bot Framework secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Microsoft Bot Framework
provider_slug: microsoft-bot-framework
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-bot-framework-activities-api-openapi.yml
  - openapi/microsoft-bot-framework-attachments-api-openapi.yml
  - openapi/microsoft-bot-framework-conversations-api-openapi.yml
  - openapi/microsoft-bot-framework-members-api-openapi.yml
  type: http
- description: Access token to authenticate calls to the Bot Connector Service.
  in: header
  name: bearer_auth
  parameter: Authorization
  sources:
  - openapi/microsoft-bot-framework-connector-api-openapi.yml
  - openapi/microsoft-bot-framework-token-api-openapi.yml
  type: apiKey
slug: microsoft-bot-framework-authentication
source_filename: microsoft-bot-framework-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-bot-framework-activities-api-openapi.yml, openapi/microsoft-bot-framework-attachments-api-openapi.yml,\n  openapi/microsoft-bot-framework-connector-api-openapi.yml, openapi/microsoft-bot-framework-conversations-api-openapi.yml,\n  openapi/microsoft-bot-framework-members-api-openapi.yml, openapi/microsoft-bot-framework-token-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-bot-framework-activities-api-openapi.yml\n  - openapi/microsoft-bot-framework-attachments-api-openapi.yml\n  - openapi/microsoft-bot-framework-conversations-api-openapi.yml\n  - openapi/microsoft-bot-framework-members-api-openapi.yml\n- name: bearer_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Access token to authenticate calls to the Bot Connector Service.\n\
  \  sources:\n  - openapi/microsoft-bot-framework-connector-api-openapi.yml\n  - openapi/microsoft-bot-framework-token-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-bot-framework/authentication/microsoft-bot-framework-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Bots
- Conversational AI
- Messaging
- Bot Framework
- Direct Line
---
