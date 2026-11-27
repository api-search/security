---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: ChatBreaker (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChatBreaker (Ingenious AI) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ChatBreaker (Ingenious AI)
provider_slug: chatbreaker-getingeniousai-com
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/admt-getingeniousai-com-openapi.json
  - openapi/agentblock-getingeniousai-com-openapi.json
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agentgate-getingeniousai-com-openapi.json
  type: http
slug: chatbreaker-getingeniousai-com-authentication
source_filename: chatbreaker-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/admt-getingeniousai-com-openapi.json, openapi/agentblock-getingeniousai-com-openapi.json,\n  openapi/agentgate-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/admt-getingeniousai-com-openapi.json\n  - openapi/agentblock-getingeniousai-com-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/agentgate-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/chatbreaker-getingeniousai-com/authentication/chatbreaker-getingeniousai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Red Teaming
- Chatbot Security
- Penetration Testing
- Automated Testing
- Security Score
- Canary Trap
---
