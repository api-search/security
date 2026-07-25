---
api_key_in: []
api_specs:
- filename: monid-openapi.json
  format: json
  label: Monid API
  slug: monid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Monid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Monid secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Monid
provider_slug: monid
scheme_count: 2
schemes:
- description: 'Monid API key (`Authorization: Bearer monid_live_...`) or a Clerk-issued JWT access token. Used for direct/server-to-server and proxy integrations.'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/monid-openapi.json
  type: http
- description: OAuth 2.0 authorization-code flow with PKCE (S256) and refresh tokens, for user-delegated access to a caller's own workspace. Issuer https://api.monid.ai; protected resource https://api.monid.ai/v1. Advertised via the anonymous /.well-known/openid-configuration + oauth-authorization-server documents.
  flows:
  - authorizationUrl: https://clerk.app.monid.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://clerk.app.monid.ai/oauth/token/revoke
    scopes:
    - openid
    - profile
    - email
    - offline_access
    - user:org:read
    tokenUrl: https://clerk.app.monid.ai/oauth/token
  name: OAuth2
  provider: Clerk (clerk.app.monid.ai)
  see: scopes/monid-scopes.yml
  sources:
  - https://api.monid.ai/.well-known/openid-configuration
  type: oauth2
slug: monid-authentication
source_filename: monid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/monid-openapi.json + https://monid.ai/docs/integrations/oauth.md + /.well-known/openid-configuration\ndocs: https://monid.ai/docs/integrations/oauth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: >-\n    Monid API key (`Authorization: Bearer monid_live_...`) or a Clerk-issued JWT\n    access token. Used for direct/server-to-server and proxy integrations.\n  sources:\n  - openapi/monid-openapi.json\n- name: OAuth2\n  type: oauth2\n  provider: Clerk (clerk.app.monid.ai)\n  description: >-\n    OAuth 2.0 authorization-code flow with PKCE (S256) and refresh tokens, for\n    user-delegated access to a caller's own workspace. Issuer https://api.monid.ai;\n    protected resource https://api.monid.ai/v1. Advertised via the anonymous\n    /.well-known/openid-configuration + oauth-authorization-server\
  \ documents.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.app.monid.ai/oauth/authorize\n    tokenUrl: https://clerk.app.monid.ai/oauth/token\n    revocationUrl: https://clerk.app.monid.ai/oauth/token/revoke\n    scopes: [openid, profile, email, offline_access, \"user:org:read\"]\n    pkce: S256\n  sources:\n  - https://api.monid.ai/.well-known/openid-configuration\n  see: scopes/monid-scopes.yml\nnotes: >-\n  Three documented integration modes: direct (single master API key), OAuth\n  (user brings their own Monid account/workspace), and proxy (self-hosted in\n  front of the API). Workspace scoping via the x-workspace-id header when an\n  OAuth/JWT token lacks org context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/authentication/monid-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Agents
- MCP
- Tools
- Data
- API Marketplace
---
