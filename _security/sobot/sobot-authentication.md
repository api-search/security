---
api_key_in: []
api_specs:
- filename: sobot-agent-api-openapi.yml
  format: yaml
  label: Sobot Agent API
  slug: sobot-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-agent-api-openapi.yml
- filename: sobot-basic-public-service-api-openapi.yml
  format: yaml
  label: Sobot basic-public/service/坐席信息管理 API
  slug: sobot-basic-public-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-basic-public-service-api-openapi.yml
- filename: sobot-exts-api-openapi.yml
  format: yaml
  label: Sobot Exts API
  slug: sobot-exts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-exts-api-openapi.yml
- filename: sobot-user-api-openapi.yml
  format: yaml
  label: Sobot User API
  slug: sobot-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-user-api-openapi.yml
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
- Chatbots
- Voice
- Ticketing
- WhatsApp
- Omnichannel
- Communications
- Artificial Intelligence
---
