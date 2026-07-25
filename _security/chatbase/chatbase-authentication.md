---
api_key_in: []
api_specs:
- filename: chatbase-chat-api-openapi.yml
  format: yaml
  label: Chatbase Chat API
  slug: chatbase-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-chat-api-openapi.yml
- filename: chatbase-chatbots-api-openapi.yml
  format: yaml
  label: Chatbase Chatbots API
  slug: chatbase-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-chatbots-api-openapi.yml
- filename: chatbase-contacts-api-openapi.yml
  format: yaml
  label: Chatbase Contacts API
  slug: chatbase-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-contacts-api-openapi.yml
- filename: chatbase-conversations-api-openapi.yml
  format: yaml
  label: Chatbase Conversations API
  slug: chatbase-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-conversations-api-openapi.yml
- filename: chatbase-leads-api-openapi.yml
  format: yaml
  label: Chatbase Leads API
  slug: chatbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-leads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chatbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chatbase
provider_slug: chatbase
scheme_count: 1
schemes:
- description: Bearer API key created in the Chatbase dashboard (Workspace Settings -> API Keys).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chatbase-openapi.yml
  type: http
slug: chatbase-authentication
source_filename: chatbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chatbase-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API key created in the Chatbase dashboard (Workspace Settings -> API Keys).\n  sources:\n  - openapi/chatbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/authentication/chatbase-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Chatbot
- AI Agent
- Customer Support
- Conversational AI
---
