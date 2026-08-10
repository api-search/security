---
api_key_in:
- header
auth_types:
- http
- oauth2
description: '1Lookup runs two distinct authentication models: a static API key presented as an HTTP Bearer token on the REST API, and OAuth 2.1 (authorization code + PKCE, with dynamic client registration) on the hosted MCP connector. Derived by hand from the published reference and the live RFC 8414 / RFC 9728 metadata — the provider publishes no OpenAPI securitySchemes to derive from mechanically.'
kind: authentication
layout: security
method: searched
name: 1Lookup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 1Lookup secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 1Lookup
provider_slug: 1lookup
scheme_count: 2
schemes:
- applies_to: https://app.1lookup.io/api/v1
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  issued_from: 1Lookup dashboard (https://app.1lookup.io) — API keys section
  name: bearerApiKey
  notes:
  - All REST requests must carry a valid API key in the Authorization header.
  - Docs advise environment-variable storage, no client-side exposure, and periodic rotation.
  - Rate limits and credit balance are enforced per organization, not per key.
  scheme: bearer
  sources:
  - https://app.1lookup.io/api
  type: http
- applies_to: https://app.1lookup.io/api/mcp
  flows:
  - authorizationUrl: https://app.1lookup.io/api/mcp/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://app.1lookup.io/api/mcp/oauth/register
    scopes:
      lookup: Access to the 1Lookup MCP tool set, billed to the authorizing account's plan credits
    tokenUrl: https://app.1lookup.io/api/mcp/oauth/token
    token_endpoint_auth_methods:
    - none
  name: mcpOAuth21
  notes:
  - No API key changes hands; the MCP client receives a scoped, revocable token.
  - Bearer token is presented in the Authorization header (bearer_methods_supported = header).
  - Access can be revoked from the 1Lookup account at any time.
  sources:
  - well-known/1lookup-oauth-authorization-server.json
  - well-known/1lookup-oauth-protected-resource.json
  type: oauth2
slug: 1lookup-authentication
source_filename: 1lookup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://app.1lookup.io/api\ndocs: https://app.1lookup.io/api\ndescription: >-\n  1Lookup runs two distinct authentication models: a static API key presented as an HTTP Bearer token on\n  the REST API, and OAuth 2.1 (authorization code + PKCE, with dynamic client registration) on the hosted\n  MCP connector. Derived by hand from the published reference and the live RFC 8414 / RFC 9728 metadata —\n  the provider publishes no OpenAPI securitySchemes to derive from mechanically.\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    applies_to: https://app.1lookup.io/api/v1\n    issued_from: 1Lookup dashboard (https://app.1lookup.io) — API keys section\n    sources: [https://app.1lookup.io/api]\n    notes:\n      - All REST\
  \ requests must carry a valid API key in the Authorization header.\n      - Docs advise environment-variable storage, no client-side exposure, and periodic rotation.\n      - Rate limits and credit balance are enforced per organization, not per key.\n  - name: mcpOAuth21\n    type: oauth2\n    applies_to: https://app.1lookup.io/api/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.1lookup.io/api/mcp/oauth/authorize\n        tokenUrl: https://app.1lookup.io/api/mcp/oauth/token\n        registrationUrl: https://app.1lookup.io/api/mcp/oauth/register\n        pkce: [S256]\n        token_endpoint_auth_methods: [none]\n        grant_types: [authorization_code, refresh_token]\n        scopes:\n          lookup: Access to the 1Lookup MCP tool set, billed to the authorizing account's plan credits\n    sources:\n      - well-known/1lookup-oauth-authorization-server.json\n      - well-known/1lookup-oauth-protected-resource.json\n    notes:\n      - No API key\
  \ changes hands; the MCP client receives a scoped, revocable token.\n      - Bearer token is presented in the Authorization header (bearer_methods_supported = header).\n      - Access can be revoked from the 1Lookup account at any time.\nplatform_controls:\n  mfa: 'Multi-factor authentication (MFA) on the dashboard — https://www.1lookup.io/security'\n  rbac: 'Role-based access control — https://www.1lookup.io/security'\n  session: 'Secure JWT with refresh tokens — https://www.1lookup.io/security'\nx-evidence:\n  - url: https://app.1lookup.io/api\n    http_status: 200\n    fetched: '2026-08-09'\n  - url: https://app.1lookup.io/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-09'\n  - url: https://www.1lookup.io/security\n    http_status: 200\n    fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1lookup/refs/heads/main/authentication/1lookup-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- phone validation
- email validation
- IP intelligence
- fraud & risk
- data enrichment
- B2B contact & company data
- SEO / web analytics
- audio transcription
- MCP / agent-native
- REST API
---
