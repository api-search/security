---
anonymous_access: false
api_key_in: []
api_specs:
- filename: api7-openapi-generated.yml
  format: yaml
  label: API7.ai API
  slug: api7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api7/refs/heads/main/openapi/_ae-authored/api7-openapi-generated.yml
auth_types: []
description: Authentication schemes documented for API7.ai AISIX gateway
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Api7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: API7.ai declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: API7.ai
provider_slug: api7
scheme_count: 5
schemes:
- evidence: 'Authorization: Bearer <secret>'
  header: Authorization
  how_to_obtain: 'Configured as the `secret` field of an agent or MCP server with `auth_type: "bearer"`.'
  location: header
  name: Bearer token (upstream)
  type: http-bearer
- evidence: 'x-api-key: <secret>'
  header: x-api-key
  how_to_obtain: 'Configured as the `secret` field of an agent or MCP server with `auth_type: "api_key"`.'
  location: header
  name: API key (upstream)
  type: apiKey
- evidence: 'Authorization: Bearer <access_token>'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: 'Configured with `auth_type: "oauth2"`, providing `client_id`, `token_url`, `secret`, and optional `scopes` in the MCP server definition.'
  location: header
  name: OAuth 2.0 client credentials (upstream)
  scopes:
  - mcp.read
  - mcp.write
  token_url: value of `token_url` field in the MCP server resource
  type: oauth2
- evidence: 'Authorization: Bearer <api key>'
  header: Authorization
  how_to_obtain: Provided as the caller's API key (`AISIX_MCP_KEY`) and sent on each request.
  location: header
  name: Gateway API key (client to AISIX)
  type: http-bearer
- evidence: 'x-api-key: <api key>'
  header: x-api-key
  how_to_obtain: Alternative to the bearer header for the caller's API key.
  location: header
  name: Gateway API key (alternative header)
  type: apiKey
slug: api7-authentication
source_filename: api7-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.api7.ai/ai-gateway/agent-gateway/upstream-authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.api7.ai/ai-gateway/agent-gateway/upstream-authentication.md\nsources:\n- https://docs.api7.ai/ai-gateway/agent-gateway/upstream-authentication.md\n- https://docs.api7.ai/ai-gateway/mcp-gateway/client-authentication.md\n- https://docs.api7.ai/ai-gateway/mcp-gateway/upstream-authentication.md\n- https://docs.api7.ai/ai-gateway/traffic-controls/caller-api-keys.md\ndescription: Authentication schemes documented for API7.ai AISIX gateway\nschemes:\n- type: http-bearer\n  name: Bearer token (upstream)\n  evidence: 'Authorization: Bearer <secret>'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Configured as the `secret` field of an agent or MCP server with `auth_type: \"bearer\"`.'\n- type: apiKey\n  name: API key (upstream)\n  evidence: 'x-api-key: <secret>'\n  location: header\n  header: x-api-key\n  how_to_obtain: 'Configured as the `secret` field of an\
  \ agent or MCP server with `auth_type: \"api_key\"`.'\n- type: oauth2\n  name: OAuth 2.0 client credentials (upstream)\n  evidence: 'Authorization: Bearer <access_token>'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: value of `token_url` field in the MCP server resource\n  scopes:\n  - mcp.read\n  - mcp.write\n  how_to_obtain: 'Configured with `auth_type: \"oauth2\"`, providing `client_id`, `token_url`, `secret`, and optional `scopes` in the MCP server\n    definition.'\n- type: http-bearer\n  name: Gateway API key (client to AISIX)\n  evidence: 'Authorization: Bearer <api key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Provided as the caller's API key (`AISIX_MCP_KEY`) and sent on each request.\n- type: apiKey\n  name: Gateway API key (alternative header)\n  evidence: 'x-api-key: <api key>'\n  location: header\n  header: x-api-key\n  how_to_obtain: Alternative to the bearer header for the caller's API key.\ndocs: https://docs.api7.ai/ai-gateway/agent-gateway/upstream-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api7/refs/heads/main/authentication/api7-authentication.yml
summary_line: 5 schemes
tags:
- Company
- API Gateway
- AI Gateway
- Open Source
- Cloud
---
