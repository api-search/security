---
api_key_in:
- header
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMind secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenMind
provider_slug: openmind
scheme_count: 3
schemes:
- applies_to: OpenMind LLM / ASR / TTS / ViLA APIs
  description: 'API key issued from the OpenMind portal, sent in the `x-api-key` header (or as `Authorization: Bearer <key>`). Keys are prefixed `om1_live_` (production) or `om1_test_` (test). For WebSocket connections the key is passed as the `api_key` query-string parameter (wss://api.openmind.com?api_key=<KEY>).'
  in: header
  name: OpenMindApiKey
  parameter: x-api-key
  sources:
  - docs
  type: apiKey
- applies_to: OpenMind LLM / ASR / TTS / ViLA APIs
  description: Same OpenMind API key accepted as an Authorization Bearer token.
  name: OpenMindApiKeyBearer
  scheme: bearer
  sources:
  - docs
  type: http
- applies_to: OpenMind Core API (api.openmind.com/api/core account & key management)
  bearerFormat: JWT
  description: 'Account and API-key management endpoints require a JWT session token issued by Clerk (clerk.com), sent as `Authorization: Bearer <JWT>`. Obtain it from the OpenMind portal session or programmatically via the Clerk SDK.'
  name: ClerkJWT
  scheme: bearer
  sources:
  - docs
  type: http
slug: openmind-authentication
source_filename: openmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.openmind.com/api-reference/introduction + https://docs.openmind.com/api-reference/introduction/account_and_key_management\ndocs: https://docs.openmind.com/api-reference/introduction/account_and_key_management\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  http_schemes: [bearer]\nschemes:\n- name: OpenMindApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: OpenMind LLM / ASR / TTS / ViLA APIs\n  description: >-\n    API key issued from the OpenMind portal, sent in the `x-api-key` header (or\n    as `Authorization: Bearer <key>`). Keys are prefixed `om1_live_` (production)\n    or `om1_test_` (test). For WebSocket connections the key is passed as the\n    `api_key` query-string parameter (wss://api.openmind.com?api_key=<KEY>).\n  sources: [docs]\n- name: OpenMindApiKeyBearer\n  type: http\n  scheme: bearer\n  applies_to: OpenMind LLM / ASR / TTS / ViLA APIs\n  description:\
  \ Same OpenMind API key accepted as an Authorization Bearer token.\n  sources: [docs]\n- name: ClerkJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: OpenMind Core API (api.openmind.com/api/core account & key management)\n  description: >-\n    Account and API-key management endpoints require a JWT session token issued\n    by Clerk (clerk.com), sent as `Authorization: Bearer <JWT>`. Obtain it from\n    the OpenMind portal session or programmatically via the Clerk SDK.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmind/refs/heads/main/authentication/openmind-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Crypto
- Robotics
- Robots
- AI
- Agents
- LLM
- ROS2
- Machine Learning
- Autonomy
---
