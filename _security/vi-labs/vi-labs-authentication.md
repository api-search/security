---
api_key_in: []
auth_types: []
description: Vi Labs publishes no developer documentation and no OpenAPI, so this profile is built entirely from the two OAuth metadata documents the vi.co host serves anonymously plus the challenge headers returned by its MCP endpoint. It describes authentication to the MCP surface on vi.co only. The enterprise platform host api.vi.co is an AWS API Gateway that returns 403 ForbiddenException to every anonymous request, publishes no metadata, and its authentication scheme is therefore unknown.
kind: authentication
layout: security
method: probed
name: Vi Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vi Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vi Labs
provider_slug: vi-labs
scheme_count: 1
schemes:
- applies_to:
  - https://vi.co/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://vi.co/oauth/authorize
  bearer_methods:
  - header
  client_registration: client_id_metadata_document_supported=true — clients identify themselves with a hosted client_id metadata document rather than pre-registration.
  evidence:
  - status: 200
    url: https://vi.co/.well-known/oauth-authorization-server
  - status: 200
    url: https://vi.co/.well-known/oauth-protected-resource
  - note: 'WWW-Authenticate: Bearer realm="https://vi.co", resource_metadata="https://vi.co/.well-known/oauth-protected-resource"'
    status: 401
    url: https://vi.co/wp-json/mcp/mcp-oauth-server
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  issuer: https://vi.co
  pkce:
    required_methods:
    - S256
  response_types:
  - code
  revocation_endpoint: https://vi.co/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://vi.co/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: vi-labs-authentication
source_filename: vi-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://vi.co/.well-known/oauth-authorization-server\nname: Vi Labs authentication profile\ndescription: >-\n  Vi Labs publishes no developer documentation and no OpenAPI, so this profile\n  is built entirely from the two OAuth metadata documents the vi.co host serves\n  anonymously plus the challenge headers returned by its MCP endpoint. It\n  describes authentication to the MCP surface on vi.co only. The enterprise\n  platform host api.vi.co is an AWS API Gateway that returns 403\n  ForbiddenException to every anonymous request, publishes no metadata, and its\n  authentication scheme is therefore unknown.\nschemes:\n- id: mcp_oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce:\n    required_methods: [S256]\n  issuer: https://vi.co\n  authorization_endpoint: https://vi.co/oauth/authorize\n  token_endpoint: https://vi.co/oauth/token\n  revocation_endpoint: https://vi.co/oauth/revoke\n  grant_types: [authorization_code,\
  \ refresh_token]\n  response_types: [code]\n  token_endpoint_auth_methods: [none]\n  scopes: [mcp]\n  client_registration: >-\n    client_id_metadata_document_supported=true — clients identify themselves\n    with a hosted client_id metadata document rather than pre-registration.\n  bearer_methods: [header]\n  applies_to:\n  - https://vi.co/wp-json/mcp/mcp-oauth-server\n  evidence:\n  - url: https://vi.co/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://vi.co/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://vi.co/wp-json/mcp/mcp-oauth-server\n    status: 401\n    note: 'WWW-Authenticate: Bearer realm=\"https://vi.co\", resource_metadata=\"https://vi.co/.well-known/oauth-protected-resource\"'\nunknown_surfaces:\n- host: api.vi.co\n  observed_status: 403\n  observed_body: '{\"message\":\"Forbidden\"}'\n  note: >-\n    AWS API Gateway (x-amzn-errortype: ForbiddenException). No WWW-Authenticate\n    header, no metadata document, no public documentation\
  \ — the authentication\n    scheme cannot be determined without a customer contract.\nstandards:\n- rfc: RFC 8414\n  name: OAuth 2.0 Authorization Server Metadata\n  observed: true\n- rfc: RFC 9728\n  name: OAuth 2.0 Protected Resource Metadata\n  observed: true\n- rfc: RFC 7636\n  name: 'PKCE (S256)'\n  observed: true\n- rfc: RFC 6750\n  name: Bearer Token Usage\n  observed: true\nx-evidence:\n  fetched: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vi-labs/refs/heads/main/authentication/vi-labs-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Health
- Healthcare
- Life Sciences
- Pharmaceuticals
- Patient Engagement
- Enterprise AI
- AI Agents
- Model Context Protocol
- Data
---
