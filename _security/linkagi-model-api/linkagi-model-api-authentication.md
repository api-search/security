---
api_key_in:
- header
api_specs:
- filename: linkagi-model-api-anthropic-style-route-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Anthropic-style route API
  slug: linkagi-model-api-anthropic-style-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-anthropic-style-route-api-openapi.yml
- filename: linkagi-model-api-discovery-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Discovery API
  slug: linkagi-model-api-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-discovery-api-openapi.yml
- filename: linkagi-model-api-gemini-style-route-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Gemini-style route API
  slug: linkagi-model-api-gemini-style-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-gemini-style-route-api-openapi.yml
- filename: linkagi-model-api-openai-compatible-api-openapi.yml
  format: yaml
  label: LinkAGI Model API OpenAI compatible API
  slug: linkagi-model-api-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-openai-compatible-api-openapi.yml
- filename: linkagi-model-api-public-metadata-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Public metadata API
  slug: linkagi-model-api-public-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-public-metadata-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Linkagi Model Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkAGI Model API secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LinkAGI Model API
provider_slug: linkagi-model-api
scheme_count: 3
schemes:
- bearerFormat: API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/linkagi-model-api-openapi.json
  type: http
- in: header
  name: anthropicApiKey
  parameter: x-api-key
  sources:
  - openapi/linkagi-model-api-openapi.json
  type: apiKey
- in: header
  name: geminiApiKey
  parameter: x-goog-api-key
  sources:
  - openapi/linkagi-model-api-openapi.json
  type: apiKey
slug: linkagi-model-api-authentication
source_filename: linkagi-model-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/linkagi-model-api-openapi.json\ndocs: https://docs.linktoagi.com/\nnote: >-\n  Static API keys minted in the New API console at https://api.linktoagi.com after email verification. No\n  OAuth, no OIDC, no SSO, no key rotation contract: GET /api/status reports oidc_enabled=false,\n  github_oauth=false, linuxdo_oauth=false, discord_oauth=false, wechat_login=false, passkey_login=false;\n  password_login_enabled=true and email_verification=true. /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server are soft-404s (SPA shell), so no scopes/ artifact is emitted.\n  The header a key travels in depends on which vendor protocol the route imitates — three schemes, one key.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  key_issuance: console (https://api.linktoagi.com) after email verification\n  group_scoping: >-\n    A key belongs to a token group (号池) that\
  \ determines which models it can address and the billing ratio\n    applied. Groups are published unauthenticated at GET /api/pricing (usable_group, group_ratio). This is\n    the closest thing LinkAGI has to a scope model.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/linkagi-model-api-openapi.json\n- name: anthropicApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/linkagi-model-api-openapi.json\n- name: geminiApiKey\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  sources:\n  - openapi/linkagi-model-api-openapi.json\nroute_map:\n- scheme: bearerAuth\n  header: 'Authorization: Bearer <key>'\n  operations: [listModels, createChatCompletion, createResponse]\n- scheme: anthropicApiKey\n  header: 'x-api-key: <key>'\n  additional_required_header: 'anthropic-version: 2023-06-01'\n  operations: [createAnthropicMessage]\n- scheme: geminiApiKey\n  header: 'x-goog-api-key: <key>'\n\
  \  operations: [generateGeminiContent]\n- scheme: none\n  operations: [getPublicStatus, getPublicPricing]\n  note: security:[] in the OpenAPI; both verified 200 anonymously on 2026-08-09\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n  - url: https://api.linktoagi.com/v1/models\n    status: 401\n    body: '{\"error\":{\"code\":\"\",\"message\":\"Invalid token (request id: ...)\",\"type\":\"new_api_error\"}}'\n  - url: https://api.linktoagi.com/api/status\n    status: 200\n  - url: https://api.linktoagi.com/.well-known/openid-configuration\n    status: 200\n    result: soft-404 (SPA shell, text/html)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/authentication/linkagi-model-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artificial Intelligence
- LLM
- AI API gateway
- relay
- OpenAI-compatible
- Anthropic-compatible
- Gemini-compatible
- Developer Tools
- CLI coding agents
- model routing
- China
---
