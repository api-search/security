---
api_key_in:
- header
api_specs:
- filename: cogny-openapi.yml
  format: yaml
  label: Cogny API
  slug: cogny-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cogny Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cogny secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cogny
provider_slug: cogny
scheme_count: 3
schemes:
- description: Bearer API key. Production keys are prefixed sk_live_, test keys sk_test_. MCP-issued anonymous keys are prefixed cogny_lite_.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cogny-openapi.yml
  type: http
- description: Legacy API-key header (equivalent to Bearer).
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/cogny-openapi.yml
  type: apiKey
- description: OAuth 2.1 (DCR + PKCE) for MCP clients.
  flows:
  - authorizationUrl: https://cogny.com/api/mcp/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://cogny.com/api/mcp/oauth/token
  name: oauth2
  sources:
  - openapi/cogny-openapi.yml
  type: oauth2
slug: cogny-authentication
source_filename: cogny-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cogny-openapi.yml\ndocs: https://cogny.com/docs/api-overview-authentication\nkey_prefixes:\n  live: sk_live_\n  test: sk_test_\n  mcp_anonymous: cogny_lite_\nagent_registration:\n  protocol: auth.md\n  register_uri: https://app.cogny.com/api/agent/auth\n  skill: https://cogny.com/auth.md\n  note: Anonymous registration returns a cogny_lite_* Bearer key in one round trip (no browser).\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API key. Production keys are prefixed sk_live_, test keys sk_test_. MCP-issued\n    anonymous keys are prefixed cogny_lite_.\n  sources:\n  - openapi/cogny-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Legacy API-key header (equivalent to Bearer).\n  sources:\n  - openapi/cogny-openapi.yml\n\
  - name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cogny.com/api/mcp/oauth/authorize\n    tokenUrl: https://cogny.com/api/mcp/oauth/token\n    scopes: 4\n  description: OAuth 2.1 (DCR + PKCE) for MCP clients.\n  sources:\n  - openapi/cogny-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/authentication/cogny-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
---
