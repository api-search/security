---
api_key_in: []
api_specs:
- filename: litmus-hiring-openapi.yml
  format: yaml
  label: Litmus Hiring REST API
  slug: litmus-hiring-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus-hiring/refs/heads/main/openapi/litmus-hiring-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Litmus Hiring Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Litmus Hiring secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Litmus Hiring
provider_slug: litmus-hiring
scheme_count: 2
schemes:
- issued_at: Dashboard -> Settings -> API Keys
  key_prefix: litmus_sk_
  location: 'Authorization: Bearer litmus_sk_...'
  name: bearerApiKey
  notes: A 401 indicates a missing, malformed, or revoked credential. Keys are production secrets; rotate regularly. Preserve trailing slashes on URLs to avoid Authorization-header drops (401) during redirects.
  scheme: bearer
  scope: organization
  sources:
  - openapi/litmus-hiring-openapi.yml
  - https://litmushiring.com/docs/rest
  surfaces:
  - rest
  - mcp
  type: http
- flows:
  - authorizationUrl: https://clerk.litmushiring.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://clerk.litmushiring.com/oauth/register
    revocationUrl: https://clerk.litmushiring.com/oauth/token/revoke
    scopes:
    - openid
    - profile
    - email
    - public_metadata
    - private_metadata
    - offline_access
    - user:org:read
    tokenUrl: https://clerk.litmushiring.com/oauth/token
  name: clerkOAuth
  provider: Clerk
  sources:
  - well-known/litmus-hiring-oauth-authorization-server.json
  surfaces:
  - mcp
  type: oauth2
slug: litmus-hiring-authentication
source_filename: litmus-hiring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://litmushiring.com/docs/rest\ndocs: https://litmushiring.com/docs/mcp/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The REST API uses an organization-scoped bearer API key. The hosted MCP\n    server additionally supports Clerk OAuth (authorization code + PKCE) for\n    interactive agent clients, and the same API key for headless automation.\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    key_prefix: litmus_sk_\n    location: 'Authorization: Bearer litmus_sk_...'\n    scope: organization\n    issued_at: Dashboard -> Settings -> API Keys\n    surfaces: [rest, mcp]\n    notes: >-\n      A 401 indicates a missing, malformed, or revoked credential. Keys are\n      production secrets; rotate regularly. Preserve trailing slashes on URLs to\n      avoid Authorization-header drops (401) during redirects.\n    sources:\
  \ [openapi/litmus-hiring-openapi.yml, https://litmushiring.com/docs/rest]\n  - name: clerkOAuth\n    type: oauth2\n    surfaces: [mcp]\n    provider: Clerk\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.litmushiring.com/oauth/authorize\n        tokenUrl: https://clerk.litmushiring.com/oauth/token\n        revocationUrl: https://clerk.litmushiring.com/oauth/token/revoke\n        registrationUrl: https://clerk.litmushiring.com/oauth/register\n        pkce: S256\n        scopes:\n          - openid\n          - profile\n          - email\n          - public_metadata\n          - private_metadata\n          - offline_access\n          - user:org:read\n    sources: [well-known/litmus-hiring-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus-hiring/refs/heads/main/authentication/litmus-hiring-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Hiring
- Recruitment
- Technical Assessment
- Developer Hiring
- MCP
- Interviewing
- Y Combinator
---
