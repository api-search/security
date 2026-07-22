---
api_key_in: []
auth_types:
- http-bearer
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rad. secures its APIs with http-bearer, apiKey, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rad.
provider_slug: rad
scheme_count: 2
schemes:
- description: 'API keys are the primary credential. Include the key as a Bearer token (Authorization: Bearer YOUR_API_KEY) on all GraphQL, MCP, and upload requests. Generated from Developer Settings.'
  key_management: https://rad.live/edit-account/?activeTab=developer
  name: BearerApiKey
  scheme: bearer
  type: http
  use_for: Direct API access, scripts, server-side integrations
- description: OAuth 2.1 with PKCE (S256) for MCP clients (Claude, Cursor, Windsurf) and third-party apps needing delegated access. Supports Dynamic Client Registration (RFC 7591) and RFC 8414 discovery.
  discovery: https://api.rad.live/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://api.rad.live/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://api.rad.live/oauth/register
    revocationUrl: https://api.rad.live/oauth/revoke
    scopes:
      mcp:tools: Access to Rad TV MCP tools
    tokenUrl: https://api.rad.live/oauth/token
  name: OAuth2
  type: oauth2
  use_for: MCP clients, third-party apps with delegated access
slug: rad-authentication
source_filename: rad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.rad.live/docs/getting-started/authentication\ndocs: https://developers.rad.live/docs/getting-started/authentication\nsummary:\n  types: [http-bearer, apiKey, oauth2]\n  transport: Authorization Bearer header on every request\n  oauth2_flows: [authorizationCode]\n  oauth2_pkce: S256\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    API keys are the primary credential. Include the key as a Bearer token\n    (Authorization: Bearer YOUR_API_KEY) on all GraphQL, MCP, and upload requests.\n    Generated from Developer Settings.\n  key_management: https://rad.live/edit-account/?activeTab=developer\n  use_for: Direct API access, scripts, server-side integrations\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.1 with PKCE (S256) for MCP clients (Claude, Cursor, Windsurf) and\n    third-party apps needing delegated access. Supports Dynamic Client\n    Registration\
  \ (RFC 7591) and RFC 8414 discovery.\n  discovery: https://api.rad.live/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rad.live/oauth/authorize\n    tokenUrl: https://api.rad.live/oauth/token\n    registrationUrl: https://api.rad.live/oauth/register\n    revocationUrl: https://api.rad.live/oauth/revoke\n    scopes:\n      mcp:tools: Access to Rad TV MCP tools\n  use_for: MCP clients, third-party apps with delegated access\nnotes:\n- All authenticated endpoints require an active subscription (Premium, Premium+, or Creator+).\n- verifyConnection query confirms auth is working and returns granted permissions.\n- endpoints:\n    graphql: POST https://api.rad.live/graphql\n    mcp: POST https://api.rad.live/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rad/refs/heads/main/authentication/rad-authentication.yml
summary_line: http-bearer/apiKey/oauth2 · 2 schemes
tags:
- Company
- Video
- Streaming
- Creator Economy
- Artificial Intelligence
- Media
- Monetization
- GraphQL
- MCP
---
