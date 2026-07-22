---
api_key_in:
- header
auth_types:
- http
description: poolside's OpenAI-compatible inference API authenticates with a bearer API key. Keys are issued by the hosted Poolside Platform (free developer access), OpenRouter, or a self-managed Poolside deployment administrator. There is no OAuth scope surface on the inference API; access is key-based.
kind: authentication
layout: security
method: searched
name: Poolside Authentication
name_suffix: Authentication
oauth_flows: []
overview: poolside secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: poolside
provider_slug: poolside
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <api-key>'
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.poolside.ai/api/overview
  type: http
slug: poolside-authentication
source_filename: poolside-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.poolside.ai/api/overview\ndocs: https://docs.poolside.ai/get-started/log-in\ndescription: >-\n  poolside's OpenAI-compatible inference API authenticates with a bearer API key.\n  Keys are issued by the hosted Poolside Platform (free developer access),\n  OpenRouter, or a self-managed Poolside deployment administrator. There is no\n  OAuth scope surface on the inference API; access is key-based.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: \"Authorization: Bearer <api-key>\"\n  sources: [https://docs.poolside.ai/api/overview]\nkey_sources:\n- name: Poolside Platform\n  url: https://platform.poolside.ai\n  note: Sign in for a free developer API key.\n- name: OpenRouter\n  url: https://openrouter.ai/poolside\n  note: Use an existing OpenRouter API key against the OpenRouter\
  \ base URL.\n- name: Poolside deployment\n  note: Self-managed on-prem / cloud deployment issues its own API tokens; login via the org sign-in system.\nci_note: >-\n  For CI/CD and automated workflows the docs recommend supplying the key via the\n  POOLSIDE_API_KEY environment variable rather than stored CLI credentials.\ncli_auth:\n  command: pool login\n  logout: pool logout\n  options: [Poolside Platform, Poolside deployment, OpenRouter, OpenAI-compatible provider]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poolside/refs/heads/main/authentication/poolside-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Coding Assistant
- Developer Tools
- LLM
- Agents
- Code Generation
- Inference
- OpenAI Compatible
---
