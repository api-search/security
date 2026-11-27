---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chinaapi-ai-openapi-generated.yml
  format: yaml
  label: ChinaAPI API
  slug: chinaapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaapi-ai/openapi/_ae-authored/chinaapi-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ChinaAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChinaAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChinaAPI
provider_slug: chinaapi-ai
scheme_count: 1
schemes:
- description: One OpenAI-compatible API key (sk-...) covers the LLM, image, video, audio and beta Social Data endpoints at https://api.chinaapi.ai/v1.
  evidence:
  - quote: 'Send `Authorization: Bearer $CHINAAPI_API_KEY`.'
    url: https://chinaapi.ai/social-data-api/docs/index.md
  - quote: create a key under Dashboard → Console → Tokens, and call supported models through the OpenAI-compatible base URL `https://api.chinaapi.ai/v1`
    url: https://chinaapi.ai/for-ai-agents/index.md
  format: 'Authorization: Bearer $CHINAAPI_API_KEY'
  header: Authorization
  in: header
  key_issuance: Keys are created under Dashboard -> Console -> Tokens after self-serve registration at https://dash.chinaapi.ai/register.
  key_prefix: sk-
  name: bearer
  scheme: bearer
  type: http
slug: chinaapi-ai-authentication
source_filename: chinaapi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: ChinaAPI authentication\ngenerated: '2026-11-03'\nmethod: searched\nsource: https://chinaapi.ai/social-data-api/docs/index.md\ndocs: https://chinaapi.ai/for-ai-agents/\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer $CHINAAPI_API_KEY'\n  key_prefix: sk-\n  description: One OpenAI-compatible API key (sk-...) covers the LLM, image, video, audio and beta Social Data endpoints at https://api.chinaapi.ai/v1.\n  key_issuance: Keys are created under Dashboard -> Console -> Tokens after self-serve registration at https://dash.chinaapi.ai/register.\n  evidence:\n  - quote: 'Send `Authorization: Bearer $CHINAAPI_API_KEY`.'\n    url: https://chinaapi.ai/social-data-api/docs/index.md\n  - quote: create a key under Dashboard → Console → Tokens, and call supported models through the OpenAI-compatible base URL `https://api.chinaapi.ai/v1`\n    url: https://chinaapi.ai/for-ai-agents/index.md\nguidance:\
  \ Keep keys server-side.\nmcp:\n  endpoint: https://api.chinaapi.ai/mcp\n  auth: none\n  note: The docs describe the MCP catalog as anonymous and read-only (\"No API key is required\").\n"
source_yaml_url: https://artifacts.apis.io/chinaapi-ai/authentication/chinaapi-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- API Gateway
- OpenAI-Compatible
- Video Generation
- Image Generation
- Speech
- MCP
- China
---
