---
api_key_in:
- header
api_specs:
- filename: archera-openapi-original.json
  format: json
  label: Archera Public API
  slug: archera-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-openapi-original.json
auth_types:
- apiKey
- oauth2
description: 'The Archera Public API supports two authentication mechanisms: a static API key sent in the x-api-key header, and OAuth 2.0 Authorization Code with PKCE (also used by the hosted MCP server, with Dynamic Client Registration).'
kind: authentication
layout: security
method: searched
name: Archera Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Archera secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Archera
provider_slug: archera
scheme_count: 2
schemes:
- description: Create an API key in the Archera web app under User Settings > API Access. Send it as the x-api-key request header. Requests are also scoped by an org_id path/query value obtained from User Settings > Organization.
  docs: https://docs.archera.ai/api-reference/public-api/api-key-access
  example: 'curl -H ''x-api-key: YOUR_API_KEY'' https://api.archera.ai/v1/org/{org_id}/metrics?provider=aws'
  in: header
  name: apiKey
  parameter_name: x-api-key
  type: apiKey
- description: OAuth 2.0 Authorization Code flow with PKCE (S256). Supports Dynamic Client Registration; token_endpoint_auth_methods_supported = none (public clients). This is the flow the hosted MCP server at https://mcp.archera.ai/mcp uses.
  docs: https://docs.archera.ai/api-reference/public-api/oauth
  flows:
  - authorizationUrl: https://api.archera.ai/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    refreshSupported: true
    registrationUrl: https://api.archera.ai/oauth/register
    revocationUrl: https://api.archera.ai/oauth/revoke
    scopes:
    - archera:read
    - archera:write
    - archera:admin
    - archera:analytics
    tokenUrl: https://api.archera.ai/oauth/token
  jwks: well-known/archera-jwks.json
  metadata: well-known/archera-oauth-authorization-server.json
  name: oauth2
  type: oauth2
slug: archera-authentication
source_filename: archera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docs.archera.ai/api-reference/public-api/api-key-access and\n  https://api.archera.ai/.well-known/oauth-authorization-server — the Archera\n  OpenAPI does not declare securitySchemes, so this profile is captured from the\n  published auth docs and live OAuth authorization-server metadata.\ndocs: https://docs.archera.ai/api-reference/public-api/api-key-access\ndescription: >-\n  The Archera Public API supports two authentication mechanisms: a static API\n  key sent in the x-api-key header, and OAuth 2.0 Authorization Code with PKCE\n  (also used by the hosted MCP server, with Dynamic Client Registration).\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Create an API key in the Archera web app under User Settings > API Access.\n    Send it as the x-api-key\
  \ request header. Requests are also scoped by an\n    org_id path/query value obtained from User Settings > Organization.\n  example: \"curl -H 'x-api-key: YOUR_API_KEY' https://api.archera.ai/v1/org/{org_id}/metrics?provider=aws\"\n  docs: https://docs.archera.ai/api-reference/public-api/api-key-access\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 Authorization Code flow with PKCE (S256). Supports Dynamic Client\n    Registration; token_endpoint_auth_methods_supported = none (public clients).\n    This is the flow the hosted MCP server at https://mcp.archera.ai/mcp uses.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.archera.ai/oauth/authorize\n    tokenUrl: https://api.archera.ai/oauth/token\n    revocationUrl: https://api.archera.ai/oauth/revoke\n    registrationUrl: https://api.archera.ai/oauth/register\n    refreshSupported: true\n    pkce: [S256]\n    scopes:\n    - archera:read\n    - archera:write\n    - archera:admin\n    - archera:analytics\n\
  \  metadata: well-known/archera-oauth-authorization-server.json\n  jwks: well-known/archera-jwks.json\n  docs: https://docs.archera.ai/api-reference/public-api/oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/authentication/archera-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Developer Tools
- FinOps
- Cloud Cost Management
- Cloud Commitments
- Cost Optimization
- MCP
- Azure
- Google Cloud
---
