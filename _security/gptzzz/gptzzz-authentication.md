---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gptzzz Authentication
name_suffix: Authentication
oauth_flows: []
overview: KaiGPT declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: KaiGPT
provider_slug: gptzzz
scheme_count: 3
schemes:
- description: 'KaiGPT API key as Authorization: Bearer <key>; the scheme the docs demonstrate for OpenAI-compatible clients.'
  evidence: https://gptzzz.ai/docs/
  name: bearerAuth
  scheme: bearer
  type: http
- description: KaiGPT API key in the x-api-key header (Anthropic Messages style), accepted per the gateway's 401 message.
  evidence: https://gptzzz.ai/v1/models (401, probed)
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  type: apiKey
- description: KaiGPT API key in the x-goog-api-key header (Gemini style), accepted per the gateway's 401 message.
  evidence: https://gptzzz.ai/v1/models (401, probed)
  in: header
  name: googApiKeyHeader
  parameter: x-goog-api-key
  type: apiKey
slug: gptzzz-authentication
source_filename: gptzzz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: KaiGPT Authentication\ngenerated: '2026-09-23'\nmethod: searched\nsource: https://gptzzz.ai/docs/\ndocs: https://gptzzz.ai/docs/\nnote: >-\n  No OpenAPI is published. The docs show only generic Bearer authentication (\"下面只演示通用 Bearer 鉴权\") with a\n  KaiGPT API key created in the console. The live gateway's anonymous 401 (probed 2026-09-23 on\n  https://gptzzz.ai/v1/models and POST https://gptzzz.ai/v1/messages) names three accepted key locations:\n  \"API key is required in Authorization header (Bearer scheme), x-api-key header, or x-goog-api-key header\".\n  The Gemini-style route https://gptzzz.ai/v1beta/models answers 401 {\"error\":{\"code\":401,\"message\":\"API key is required\",\"status\":\"UNAUTHENTICATED\"}}.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'KaiGPT API key as Authorization: Bearer <key>; the scheme the docs demonstrate for OpenAI-compatible clients.'\n  evidence: https://gptzzz.ai/docs/\n- name: apiKeyHeader\n  type:\
  \ apiKey\n  in: header\n  parameter: x-api-key\n  description: KaiGPT API key in the x-api-key header (Anthropic Messages style), accepted per the gateway's 401 message.\n  evidence: https://gptzzz.ai/v1/models (401, probed)\n- name: googApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  description: KaiGPT API key in the x-goog-api-key header (Gemini style), accepted per the gateway's 401 message.\n  evidence: https://gptzzz.ai/v1/models (401, probed)\nkey_handling: >-\n  Docs: keep the key only in server-side secret management or local environment variables; never in front-end code,\n  screenshots, public repos, email or tickets; support only accepts masked prefixes/suffixes such as sk-abcd…wxyz.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gptzzz/refs/heads/main/authentication/gptzzz-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- LLM Gateway
- API Relay
- OpenAI-Compatible
- Claude
- Gemini
- LLM
- China
---
