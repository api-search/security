---
api_key_in:
- header
api_specs:
- filename: evermuse-ingest-v1-openapi-original.yml
  format: yaml
  label: Evermuse Ingestion API
  slug: evermuse-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/openapi/evermuse-ingest-v1-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Evermuse Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Evermuse secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Evermuse
provider_slug: evermuse
scheme_count: 2
schemes:
- description: 'Workspace-scoped API key, sent as the `x-api-key` header. Keys are prefixed

    `em_sk_` and created in Settings > API Keys. Each workspace can hold up to 10 keys.

    The Ingestion API requires the `api:write` permission (`api:read` keys get 403).'
  in: header
  name: IngestApiKey
  parameter: x-api-key
  sources:
  - openapi/evermuse-ingest-v1-openapi-original.yml
  - https://docs.evermuse.com/authentication
  type: apiKey
- description: 'OAuth 2.1 protects the hosted Evermuse MCP server (https://api.evermuse.com/api/mcp).

    Authorization Server metadata is published at

    /.well-known/oauth-authorization-server (RFC 8414) and the protected resource at

    /.well-known/oauth-protected-resource (RFC 9728). PKCE (S256) is required and

    Dynamic Client Registration is supported (RFC 7591) at /oauth/register.'
  flows:
  - authorizationUrl: https://api.evermuse.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.evermuse.com/oauth/register
    scopes:
    - mcp:read
    - mcp:write
    - mcp:thirdparty
    tokenUrl: https://api.evermuse.com/oauth/token
  name: EvermuseOAuth
  scheme: authorization_code
  sources:
  - well-known/evermuse-oauth-authorization-server.json
  - well-known/evermuse-oauth-protected-resource.json
  type: oauth2
slug: evermuse-authentication
source_filename: evermuse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/evermuse-ingest-v1-openapi-original.yml\ndocs: https://docs.evermuse.com/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: IngestApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Workspace-scoped API key, sent as the `x-api-key` header. Keys are prefixed\n    `em_sk_` and created in Settings > API Keys. Each workspace can hold up to 10 keys.\n    The Ingestion API requires the `api:write` permission (`api:read` keys get 403).\n  sources:\n  - openapi/evermuse-ingest-v1-openapi-original.yml\n  - https://docs.evermuse.com/authentication\n- name: EvermuseOAuth\n  type: oauth2\n  scheme: authorization_code\n  description: |-\n    OAuth 2.1 protects the hosted Evermuse MCP server (https://api.evermuse.com/api/mcp).\n    Authorization Server metadata is published at\n    /.well-known/oauth-authorization-server\
  \ (RFC 8414) and the protected resource at\n    /.well-known/oauth-protected-resource (RFC 9728). PKCE (S256) is required and\n    Dynamic Client Registration is supported (RFC 7591) at /oauth/register.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.evermuse.com/oauth/authorize\n    tokenUrl: https://api.evermuse.com/oauth/token\n    registrationUrl: https://api.evermuse.com/oauth/register\n    pkce: S256\n    scopes:\n    - mcp:read\n    - mcp:write\n    - mcp:thirdparty\n  sources:\n  - well-known/evermuse-oauth-authorization-server.json\n  - well-known/evermuse-oauth-protected-resource.json\npermissions:\n- key: api:read\n  description: Read access to API endpoints (e.g. checking batch status).\n- key: api:write\n  description: Write access to API endpoints. Required for the Ingestion API.\n- key: mcp:read\n  description: Read access via MCP. Requires a default product.\n- key: mcp:write\n  description: Write access via MCP. Requires a default product.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/authentication/evermuse-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Product Management
- Customer Feedback
- Voice of Customer
- Artificial Intelligence
- Data Ingestion
- Product Analytics
- MCP
- Developer Tools
---
