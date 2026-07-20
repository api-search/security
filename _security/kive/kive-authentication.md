---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kive secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kive
provider_slug: kive
scheme_count: 1
schemes:
- bearer:
    methods:
    - header
    protected_resource: https://mcp.kive.ai/mcp
  flows:
  - authorizationUrl: https://mcp.kive.ai/oauth/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    refreshSupported: true
    revocationUrl: https://mcp.kive.ai/oauth/revoke
    scopes:
      kive:mcp: Access the Kive MCP server on behalf of the authorizing user
      offline_access: Obtain a refresh token for long-lived access
    tokenUrl: https://mcp.kive.ai/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://mcp.kive.ai
  name: KiveMCPOAuth
  source: https://mcp.kive.ai/.well-known/oauth-authorization-server
  type: oauth2
slug: kive-authentication
source_filename: kive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.kive.ai/.well-known/oauth-authorization-server\ndocs: https://kive.ai/docs/mcp/connect-any-client.md\nnotes: >-\n  Kive publishes no public REST API and therefore no OpenAPI securitySchemes.\n  Its one programmable surface is the Kive MCP server, protected by OAuth 2.1\n  with PKCE. Authorization is user-driven: an MCP client is redirected to Kive,\n  the user signs in and approves workspace access, and the resulting token\n  carries that user's workspace permissions and credit entitlement.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: KiveMCPOAuth\n  type: oauth2\n  source: https://mcp.kive.ai/.well-known/oauth-authorization-server\n  issuer: https://mcp.kive.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.kive.ai/oauth/authorize\n    tokenUrl: https://mcp.kive.ai/oauth/token\n    revocationUrl: https://mcp.kive.ai/oauth/revoke\n\
  \    refreshSupported: true\n    pkce_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    scopes:\n      kive:mcp: Access the Kive MCP server on behalf of the authorizing user\n      offline_access: Obtain a refresh token for long-lived access\n  bearer:\n    methods: [header]\n    protected_resource: https://mcp.kive.ai/mcp\nrevocation:\n  user_facing: Settings -> MCP -> Apps -> Revoke\n  endpoint: https://mcp.kive.ai/oauth/revoke\n  notes: Revoking from Kive is the authoritative disconnect; it immediately stops\n    the client reading from or spending credits in the workspace.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kive/refs/heads/main/authentication/kive-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- SaaS
- Artificial Intelligence
- Generative AI
- Creative
- Product Photography
- Digital Asset Management
- E-Commerce
- Images
- Video
- MCP
---
