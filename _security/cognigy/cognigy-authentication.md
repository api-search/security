---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cognigy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognigy secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cognigy
provider_slug: cognigy
scheme_count: 3
schemes:
- description: Primary authentication for the Cognigy.AI REST API. Pass your personal API key in the X-API-Key request header. API keys are generated from user profile settings in the Cognigy.AI management UI.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - docs
  type: apiKey
- description: Alternative authentication for the Cognigy.AI REST API — the same API key may be supplied as an api_key query-string parameter instead of the X-API-Key header.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - docs
  type: apiKey
- description: Short-lived access tokens can be created via the token endpoints (api-reference/tokens/create-a-token) for scoped, time-limited API access.
  name: token
  scheme: bearer
  sources:
  - docs
  type: http
slug: cognigy-authentication
source_filename: cognigy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cognigy.com/ai/for-developers/developers/api-and-cli/\ndocs: https://docs.cognigy.com/api-reference/management-ui/create-an-api-key/\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Primary authentication for the Cognigy.AI REST API. Pass your personal API key\n    in the X-API-Key request header. API keys are generated from user profile\n    settings in the Cognigy.AI management UI.\n  sources: [docs]\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    Alternative authentication for the Cognigy.AI REST API — the same API key may\n    be supplied as an api_key query-string parameter instead of the X-API-Key header.\n  sources: [docs]\n- name: token\n  type: http\n  scheme: bearer\n  description: >-\n    Short-lived access tokens can be\
  \ created via the token endpoints\n    (api-reference/tokens/create-a-token) for scoped, time-limited API access.\n  sources: [docs]\nnotes:\n- The Webhook Endpoint additionally supports an optional X-Webhook-Key header for\n  requests sent into Cognigy, and optional HTTP Basic Auth for callbacks Cognigy\n  sends to your webhook URL.\n- The API is region/environment-scoped; the API key is only valid against the base\n  URL of the environment where it was issued (Trial, SaaS App, on-prem, or NiCE CXone).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognigy/refs/heads/main/authentication/cognigy-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Conversational AI
- Agentic AI
- Contact Center
- Customer Service Automation
- Chatbots
- Voice AI
- Virtual Agents
- Enterprise AI
- Omnichannel
---
