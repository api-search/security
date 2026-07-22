---
api_key_in:
- header
api_specs:
- filename: nexosai-gateway-openapi-original.yml
  format: yaml
  label: nexos.ai Gateway API
  slug: nexosai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-gateway-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nexosai Authentication
name_suffix: Authentication
oauth_flows: []
overview: nexos.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: nexos.ai
provider_slug: nexosai
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nexosai-gateway-openapi-original.yml
  type: http
- description: 'Authenticate by sending your nexos API key in the `X-Api-Key` header (e.g. `X-Api-Key: nexos-...` for a user key or `X-Api-Key: nexos-team-...` for a team key). This is an alternative to the `Authorization: Bearer` scheme. If both `X-Nexos-Key` and `X-Api-Key` are sent, `X-Nexos-Key` takes precedence.'
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/nexosai-gateway-openapi-original.yml
  type: apiKey
slug: nexosai-authentication
source_filename: nexosai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nexosai-gateway-openapi-original.yml\ndocs: https://docs.nexos.ai/gateway-api/api-keys\nkey_prefixes:\n  user: nexos-\n  team: nexos-team-\nrequirements: API usage requires both a paid subscription and separately purchased API credits.\nrotation: API keys can be rotated in the API Keys settings; the old key is deprecated on rotation.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nexosai-gateway-openapi-original.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Authenticate by sending your nexos API key in the `X-Api-Key` header (e.g. `X-Api-Key:\n    nexos-...` for a user key or `X-Api-Key: nexos-team-...` for a team key). This is an alternative\n    to the `Authorization: Bearer` scheme. If both `X-Nexos-Key` and `X-Api-Key` are sent, `X-Nexos-Key`\n    takes precedence.'\n\
  \  sources:\n  - openapi/nexosai-gateway-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/authentication/nexosai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Machine Learning
- Embeddings
- Agents
- Developer Tools
- OpenAI Compatible
---
