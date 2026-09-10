---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Motomarks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Motomarks declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Motomarks
provider_slug: motomarks
scheme_count: 3
schemes:
- description: 'Secret keys (sk_...) are server-side only, sent as "Authorization: Bearer YOUR_SECRET_KEY". They authenticate the JSON API (api.motomarks.io) and headless connections to the MCP server. Full account access; never for client-side code.'
  id: secret-key-bearer
  key_prefix: sk_
  scheme: bearer
  surfaces:
  - JSON API
  - MCP Server (headless)
  type: http
- description: Publishable keys (pk_...) are safe to expose client-side and authenticate the Image CDN as a ?token= query parameter. On Pro and Enterprise plans each publishable key can carry a hostname allowlist (Origin/Referer-checked domain restrictions; wildcard subdomains supported; localhost always permitted).
  id: publishable-key-token
  in: query
  key_prefix: pk_
  name: token
  surfaces:
  - Image CDN
  type: apiKey
- description: OAuth 2.1 authorization-code with PKCE (S256) and dynamic client registration (registration_endpoint published) per the MCP authorization spec. Discovery via /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource on motomarks.io (both HTTP 200, saved under well-known/).
  flows:
    authorizationCode:
      authorizationUrl: https://motomarks.io/api/auth/mcp/authorize
      refreshUrl: https://motomarks.io/api/auth/mcp/token
      scopes:
        email: Email address
        offline_access: Refresh tokens
        openid: OpenID Connect identity
        profile: Basic profile
      tokenUrl: https://motomarks.io/api/auth/mcp/token
  id: oauth2
  surfaces:
  - MCP Server
  type: oauth2
slug: motomarks-authentication
source_filename: motomarks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Motomarks Authentication\ngenerated: '2026-09-09'\nmethod: searched\nsource: https://motomarks.io/docs/platform/api-keys\ndocs: https://motomarks.io/docs/platform/api-keys\nnote: >-\n  No OpenAPI is published; profile assembled from the API-keys, API-reference and MCP docs plus live probes of\n  the OAuth discovery documents and the gated API host (api.motomarks.io answers 403 {\"error\":\"invalid_token\"}\n  without a key).\nschemes:\n  - id: secret-key-bearer\n    type: http\n    scheme: bearer\n    key_prefix: sk_\n    surfaces: [JSON API, MCP Server (headless)]\n    description: >-\n      Secret keys (sk_...) are server-side only, sent as \"Authorization: Bearer YOUR_SECRET_KEY\". They\n      authenticate the JSON API (api.motomarks.io) and headless connections to the MCP server. Full account\n      access; never for client-side code.\n  - id: publishable-key-token\n    type: apiKey\n    in: query\n    name: token\n    key_prefix: pk_\n    surfaces: [Image CDN]\n\
  \    description: >-\n      Publishable keys (pk_...) are safe to expose client-side and authenticate the Image CDN as a ?token=\n      query parameter. On Pro and Enterprise plans each publishable key can carry a hostname allowlist\n      (Origin/Referer-checked domain restrictions; wildcard subdomains supported; localhost always permitted).\n  - id: oauth2\n    type: oauth2\n    surfaces: [MCP Server]\n    flows:\n      authorizationCode:\n        authorizationUrl: https://motomarks.io/api/auth/mcp/authorize\n        tokenUrl: https://motomarks.io/api/auth/mcp/token\n        refreshUrl: https://motomarks.io/api/auth/mcp/token\n        scopes:\n          openid: OpenID Connect identity\n          profile: Basic profile\n          email: Email address\n          offline_access: Refresh tokens\n    description: >-\n      OAuth 2.1 authorization-code with PKCE (S256) and dynamic client registration (registration_endpoint\n      published) per the MCP authorization spec. Discovery via /.well-known/oauth-authorization-server\
  \ and\n      /.well-known/oauth-protected-resource on motomarks.io (both HTTP 200, saved under well-known/).\noptional_headers:\n  - name: X-Motomarks-Referer\n    description: Optional analytics-only attribution of server-side requests to a site or app; never access control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motomarks/refs/heads/main/authentication/motomarks-authentication.yml
summary_line: 3 schemes
tags:
- automotive
- logo
- image-cdn
- manufacturer
- brand-assets
- images
- CDN
- developer-tools
- agent-native
- MCP
- reference-data
---
