---
api_key_in:
- header
api_specs:
- filename: seltz-openapi-original.json
  format: json
  label: Seltz Web Knowledge API
  slug: seltz-web-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seltz/refs/heads/main/openapi/seltz-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Seltz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seltz secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Seltz
provider_slug: seltz
scheme_count: 2
schemes:
- description: Seltz API key passed in the x-api-key request header. Generate keys in the console at https://console.seltz.ai/api-keys. The REST /v1/search and /v1/answer endpoints also accept the key in the JSON body as `api_key`, but the x-api-key header takes precedence and is the recommended method.
  in: header
  name: ApiKeyHeader
  parameter_name: x-api-key
  sources:
  - openapi/seltz-openapi-original.json
  type: apiKey
- description: 'The hosted MCP server (https://mcp.seltz.ai/mcp) authenticates with the same API key passed as `Authorization: Bearer <SELTZ_API_KEY>`.'
  name: BearerToken
  scheme: bearer
  sources:
  - mcp/seltz-mcp.yml
  type: http
slug: seltz-authentication
source_filename: seltz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.seltz.ai/quickstart\ndocs: https://docs.seltz.ai/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Seltz API key passed in the x-api-key request header. Generate keys in the\n    console at https://console.seltz.ai/api-keys. The REST /v1/search and\n    /v1/answer endpoints also accept the key in the JSON body as `api_key`, but\n    the x-api-key header takes precedence and is the recommended method.\n  sources: [openapi/seltz-openapi-original.json]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    The hosted MCP server (https://mcp.seltz.ai/mcp) authenticates with the same\n    API key passed as `Authorization: Bearer <SELTZ_API_KEY>`.\n  sources: [mcp/seltz-mcp.yml]\nnotes: >-\n  The published OpenAPI (v1.3.0) models the API key as a required\
  \ `x-api-key`\n  header parameter rather than a formal components.securitySchemes entry, so\n  the mechanical auth-derive script found no schemes; this profile is captured\n  from the documentation and spec parameters. No OAuth2/OIDC flows exist, so\n  there is no scopes artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seltz/refs/heads/main/authentication/seltz-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Web Search
- AI Infrastructure
- Retrieval
- RAG
- Agents
- LLM
- Knowledge API
- Developer Tools
- MCP
---
