---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Airops Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AirOps secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AirOps
provider_slug: airops
scheme_count: 2
schemes:
- applies_to: https://api.airops.com/public_api/*
  description: Workspace API key presented as a Bearer token in the Authorization header for the REST API at api.airops.com. Keys are created and regenerated in Workspace Settings; regenerating immediately invalidates the previous key. Some execute endpoints also accept the key as an auth_token query parameter (webhook flows).
  format: Bearer [example key]
  header: Authorization
  location: header
  name: apiKeyBearer
  scheme: bearer
  type: http
- applies_to: https://app.airops.com/mcp
  description: OAuth 2.0 authorization-code flow (PKCE S256) used by the hosted MCP server at app.airops.com/mcp and OAuth clients. Discovery published at app.airops.com/.well-known/openid-configuration and /oauth-authorization-server.
  flows:
  - authorizationUrl: https://app.airops.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://app.airops.com/oauth/introspect
    pkce:
    - S256
    revocationUrl: https://app.airops.com/oauth/revoke
    scopes_supported:
    - api
    - openid
    - profile
    - email
    tokenUrl: https://app.airops.com/oauth/token
    userinfoUrl: https://app.airops.com/oauth/userinfo
  name: oauth2
  scheme: authorizationCode
  type: oauth2
slug: airops-authentication
source_filename: airops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.airops.com/api-reference/using-the-api/authentication\ndocs: https://docs.airops.com/api-reference/using-the-api/authentication\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Bearer [example key]'\n  description: >-\n    Workspace API key presented as a Bearer token in the Authorization header for\n    the REST API at api.airops.com. Keys are created and regenerated in Workspace\n    Settings; regenerating immediately invalidates the previous key. Some execute\n    endpoints also accept the key as an auth_token query parameter (webhook flows).\n  applies_to: https://api.airops.com/public_api/*\n- name: oauth2\n  type: oauth2\n  scheme: authorizationCode\n  description: >-\n    OAuth 2.0 authorization-code flow (PKCE S256)\
  \ used by the hosted MCP server at\n    app.airops.com/mcp and OAuth clients. Discovery published at\n    app.airops.com/.well-known/openid-configuration and /oauth-authorization-server.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.airops.com/oauth/authorize\n    tokenUrl: https://app.airops.com/oauth/token\n    revocationUrl: https://app.airops.com/oauth/revoke\n    introspectionUrl: https://app.airops.com/oauth/introspect\n    userinfoUrl: https://app.airops.com/oauth/userinfo\n    scopes_supported: [api, openid, profile, email]\n    pkce: [S256]\n  applies_to: https://app.airops.com/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/authentication/airops-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Applications
- AI
- Content
- SEO
- AEO
- Answer Engine Optimization
- Generative Engine Optimization
- Workflows
- MCP
- Analytics
---
