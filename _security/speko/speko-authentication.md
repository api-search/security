---
api_key_in: []
api_specs:
- filename: speko-agents-api-openapi.yml
  format: yaml
  label: Speko Agents API
  slug: speko-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-agents-api-openapi.yml
- filename: speko-providers-api-openapi.yml
  format: yaml
  label: Speko Providers API
  slug: speko-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-providers-api-openapi.yml
- filename: speko-telephony-api-openapi.yml
  format: yaml
  label: Speko Telephony API
  slug: speko-telephony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-telephony-api-openapi.yml
- filename: speko-voice-api-openapi.yml
  format: yaml
  label: Speko Voice API
  slug: speko-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-voice-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Speko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speko secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Speko
provider_slug: speko
scheme_count: 1
schemes:
- bearerFormat: API key (sk_live_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/speko-openapi-original.json
  type: http
slug: speko-authentication
source_filename: speko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/speko-openapi-original.json\ndocs: https://docs.speko.dev/api-reference/introduction\nnotes: >-\n  Single auth model - a bearer API key (sk_live_...) sent as Authorization:\n  Bearer. Keys are minted in the platform dashboard (https://platform.speko.dev).\n  The hosted MCP server additionally supports OAuth. No OAuth2 flows in the REST API.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (sk_live_...)\n  sources:\n  - openapi/speko-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/authentication/speko-authentication.yml
summary_line: http · 1 scheme
tags:
- Voice
- Voice AI
- Speech-to-Text
- Text to Speech
- LLM
- Telephony
- API Gateway
- Conversational AI
- Developer Tools
- AI Infrastructure
---
