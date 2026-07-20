---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Instawork Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instawork secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instawork
provider_slug: instawork
scheme_count: 1
schemes:
- authorizationUrl: https://finch.instawork.com/mcp/partner/authorize
  bearer_methods_supported:
  - header
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://finch.instawork.com/mcp/partner
  name: OAuth2
  registrationUrl: https://finch.instawork.com/mcp/partner/register
  scopes:
  - description: Read access to partner staffing data (locations, positions, pricing, templates, shift groups)
    scope: read
  - description: Create draft and confirmed shift bookings on behalf of the partner
    scope: write
  sources:
  - well-known/instawork-oauth-authorization-server.json
  tokenUrl: https://finch.instawork.com/mcp/partner/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: instawork-authentication
source_filename: instawork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://finch.instawork.com/.well-known/oauth-authorization-server/mcp/partner\ndocs: https://github.com/instawork/skills/blob/main/skills/find-workers/setup.md\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  scopes: [read, write]\n  notes: >-\n    Authentication to the Instawork Partner MCP server is OAuth 2.1 with PKCE\n    (S256) and dynamic client registration (RFC 7591). Partners log in with\n    their Instawork business-partner credentials and grant consent on first use.\n    No public REST API or API-key surface is documented; the MCP server is the\n    partner integration surface.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    issuer: https://finch.instawork.com/mcp/partner\n    authorizationUrl: https://finch.instawork.com/mcp/partner/authorize\n    tokenUrl: https://finch.instawork.com/mcp/partner/token\n    registrationUrl: https://finch.instawork.com/mcp/partner/register\n\
  \    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    scopes:\n      - scope: read\n        description: Read access to partner staffing data (locations, positions, pricing, templates, shift groups)\n      - scope: write\n        description: Create draft and confirmed shift bookings on behalf of the partner\n    bearer_methods_supported: [header]\n    sources: [well-known/instawork-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instawork/refs/heads/main/authentication/instawork-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketplace
- Staffing
- Gig Economy
- Hospitality
- Workforce
- Labor
- MCP
- Agent
---
