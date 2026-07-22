---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pointfive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pointfive secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pointfive
provider_slug: pointfive
scheme_count: 1
schemes:
- bearer_methods:
  - header
  flows:
  - authorizationUrl: https://mcp.pointfive.co/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://mcp.pointfive.co/register
    revocationUrl: https://mcp.pointfive.co/revoke
    scopes:
      api:read: Read access to PointFive data (opportunities, resources, anomalies, commitments).
      api:write: Write access to PointFive data.
    tokenUrl: https://mcp.pointfive.co/token
    token_endpoint_auth_methods:
    - none
  name: OAuth2
  profile: OAuth 2.1
  sources:
  - well-known/pointfive-oauth-authorization-server.json
  type: oauth2
slug: pointfive-authentication
source_filename: pointfive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.pointfive.co/.well-known/oauth-authorization-server\ndocs: https://www.pointfive.co/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    PointFive's public programmatic surface is its MCP server, which authenticates\n    with OAuth 2.1 (authorization code + PKCE S256, refresh tokens, dynamic client\n    registration). Users only access data they can already see in the PointFive\n    platform. The core web application (app.pointfive.co) is a separate\n    session/SSO-based login; no first-party REST API is publicly documented.\nschemes:\n- name: OAuth2\n  type: oauth2\n  profile: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.pointfive.co/authorize\n    tokenUrl: https://mcp.pointfive.co/token\n    registrationUrl: https://mcp.pointfive.co/register\n    revocationUrl: https://mcp.pointfive.co/revoke\n    pkce: S256\n    grant_types: [authorization_code,\
  \ refresh_token]\n    token_endpoint_auth_methods: [none]\n    scopes:\n      api:read: Read access to PointFive data (opportunities, resources, anomalies, commitments).\n      api:write: Write access to PointFive data.\n  bearer_methods: [header]\n  sources: [well-known/pointfive-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointfive/refs/heads/main/authentication/pointfive-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cloud Saas
- FinOps
- Cloud Cost Optimization
- Cloud Infrastructure
- Kubernetes
- AI Infrastructure
- MCP
---
