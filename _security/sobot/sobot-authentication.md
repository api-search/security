---
api_key_in: []
api_specs:
- filename: sobot-online-openapi.json
  format: json
  label: Sobot Online Chat API
  slug: sobot-online-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-online-openapi.json
- filename: sobot-basic-openapi.json
  format: json
  label: Sobot Basic (Agent) API
  slug: sobot-basic-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-basic-openapi.json
- filename: sobot-voice-openapi.json
  format: json
  label: Sobot Voice Extension API
  slug: sobot-voice-extension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-voice-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sobot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sobot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sobot
provider_slug: sobot
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sobot-basic-openapi.json
  - openapi/sobot-main-openapi.json
  - openapi/sobot-online-openapi.json
  - openapi/sobot-voice-openapi.json
  type: http
slug: sobot-authentication
source_filename: sobot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sobot-basic-openapi.json, openapi/sobot-main-openapi.json, openapi/sobot-online-openapi.json,\n  openapi/sobot-voice-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sobot-basic-openapi.json\n  - openapi/sobot-main-openapi.json\n  - openapi/sobot-online-openapi.json\n  - openapi/sobot-voice-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/authentication/sobot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Contact Center
- Customer Service
- Live Chat
- Chatbot
- Voice
- Ticketing
- WhatsApp
- Omnichannel
- Communications
- Artificial Intelligence
---
