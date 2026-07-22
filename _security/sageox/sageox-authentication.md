---
api_key_in: []
api_specs:
- filename: sageox-openapi-original.json
  format: json
  label: SageOx API
  slug: sageox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/openapi/sageox-openapi-original.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sageox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SageOx secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SageOx
provider_slug: sageox
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT token obtained from the auth service (/api/auth/token).

    Token is validated using JWKS from the auth service (https://sageox.ai/api/auth/jwks).

    Required claims: sub (user_id), email, name, tier.

    All REST API endpoints require: Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sageox-openapi-original.json
  type: http
- description: OAuth 2.0 / OpenID Connect authorization server (Better Auth). Advertised via /.well-known/oauth-authorization-server and /.well-known/openid-configuration. Used for the MCP server's scoped grants and third-party client authorization.
  flows:
  - authorizationUrl: https://sageox.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    jwksUri: https://sageox.ai/api/auth/jwks
    pkce: S256
    registrationUrl: https://sageox.ai/api/auth/oauth2/register
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://sageox.ai/api/auth/oauth2/token
    userinfoUrl: https://sageox.ai/api/auth/oauth2/userinfo
  name: oauth2
  sources:
  - well-known/sageox-openid-configuration.json
  - well-known/sageox-oauth-authorization-server.json
  type: oauth2
slug: sageox-authentication
source_filename: sageox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sageox-openapi-original.json\ndocs: https://sageox.ai/docs\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT token obtained from the auth service (/api/auth/token).\n    Token is validated using JWKS from the auth service (https://sageox.ai/api/auth/jwks).\n    Required claims: sub (user_id), email, name, tier.\n    All REST API endpoints require: Authorization: Bearer <token>.\n  sources:\n  - openapi/sageox-openapi-original.json\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 / OpenID Connect authorization server (Better Auth). Advertised via\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration.\n    Used for the MCP server's scoped grants and third-party client authorization.\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://sageox.ai/api/auth/oauth2/authorize\n    tokenUrl: https://sageox.ai/api/auth/oauth2/token\n    userinfoUrl: https://sageox.ai/api/auth/oauth2/userinfo\n    registrationUrl: https://sageox.ai/api/auth/oauth2/register\n    jwksUri: https://sageox.ai/api/auth/jwks\n    pkce: S256\n    scopes:\n    - openid\n    - profile\n    - email\n    - offline_access\n  sources:\n  - well-known/sageox-openid-configuration.json\n  - well-known/sageox-oauth-authorization-server.json\ncli_auth:\n  description: >-\n    The Ox CLI uses a device-authorization flow — it initiates a device flow to\n    obtain initial credentials, exchanges the device code for a JWT, stores it\n    securely, and refreshes when expired.\n  source: openapi/sageox-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/authentication/sageox-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Company
- AI Agents
- Developer Tools
- Knowledge Management
- Agent Memory
- Model Context Protocol
- MCP
- CLI
- Team Collaboration
- Agentic Engineering
---
