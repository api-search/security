---
api_key_in: []
api_specs:
- filename: talkable-v2-openapi-original.yml
  format: yaml
  label: Talkable API v2
  slug: talkable-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-v2-openapi-original.yml
- filename: talkable-webhooks-openapi-original.yml
  format: yaml
  label: Talkable Webhooks
  slug: talkable-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-webhooks-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Talkable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Talkable secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Talkable
provider_slug: talkable
scheme_count: 3
schemes:
- applies_to: REST API v2
  description: REST API v2 authentication. Provide your Talkable API key as a Bearer token in the Authorization header. The API key is managed in Site Settings -> API Integration -> API Key (also in Account Settings). Do not embed the key in browser-side JavaScript.
  example: 'Authorization: Bearer <API_KEY>'
  name: api_key
  scheme: bearer
  sources:
  - openapi/talkable-v2-openapi-original.yml
  type: http
- applies_to: MCP server
  description: MCP server authentication. OAuth 2.1 with PKCE (S256) and Dynamic Client Registration (RFC 7591). Talkable is both authorization server and resource server; clients self-configure from the well-known discovery documents.
  docs: https://docs.talkable.com/mcp_server/authentication/
  flows:
  - authorizationUrl: https://www.talkable.com/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://www.talkable.com/oauth/register
    scopes:
      mcp:read: Read account and site data over MCP.
      mcp:write: Create or update Talkable data over MCP.
    tokenUrl: https://www.talkable.com/oauth/token
  name: oauth2
  sources:
  - well-known/talkable-oauth-authorization-server.json
  type: oauth2
- applies_to: MCP server
  description: Long-lived personal (or scoped account/site) API key usable as a Bearer token against the MCP endpoint. Created under My Profile -> API Keys.
  name: mcp_personal_api_key
  scheme: bearer
  type: http
slug: talkable-authentication
source_filename: talkable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.talkable.com/api_v2/intro/ + openapi/talkable-v2-openapi-original.yml\ndocs: https://docs.talkable.com/api_v2/intro/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: api_key\n    type: http\n    scheme: bearer\n    description: >-\n      REST API v2 authentication. Provide your Talkable API key as a Bearer\n      token in the Authorization header. The API key is managed in\n      Site Settings -> API Integration -> API Key (also in Account Settings).\n      Do not embed the key in browser-side JavaScript.\n    example: 'Authorization: Bearer <API_KEY>'\n    sources: [openapi/talkable-v2-openapi-original.yml]\n    applies_to: REST API v2\n  - name: oauth2\n    type: oauth2\n    description: >-\n      MCP server authentication. OAuth 2.1 with PKCE (S256) and Dynamic Client\n      Registration (RFC 7591). Talkable is both authorization server and\n\
  \      resource server; clients self-configure from the well-known discovery\n      documents.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.talkable.com/oauth/authorize\n        tokenUrl: https://www.talkable.com/oauth/token\n        registrationUrl: https://www.talkable.com/oauth/register\n        scopes:\n          mcp:read: Read account and site data over MCP.\n          mcp:write: Create or update Talkable data over MCP.\n    sources: [well-known/talkable-oauth-authorization-server.json]\n    applies_to: MCP server\n    docs: https://docs.talkable.com/mcp_server/authentication/\n  - name: mcp_personal_api_key\n    type: http\n    scheme: bearer\n    description: >-\n      Long-lived personal (or scoped account/site) API key usable as a Bearer\n      token against the MCP endpoint. Created under My Profile -> API Keys.\n    applies_to: MCP server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/authentication/talkable-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Referral Marketing
- Loyalty
- Marketing
- E-commerce
- Advocacy
- Rewards
- Customer Acquisition
- Webhooks
- MCP
---
