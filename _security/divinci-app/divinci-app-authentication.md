---
anonymous_access: false
api_key_in: []
api_specs:
- filename: divinci-app-api-openapi.yml
  format: yaml
  label: Divinci AI API API
  slug: divinci-ai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/divinci-app/openapi/_original/divinci-app-api-openapi.yml
auth_types: []
description: Divinci agents authenticate using OAuth 2.1 with dynamic client registration and the authorization code flow (PKCE). The access token is sent in the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Divinci App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Divinci declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Divinci
provider_slug: divinci-app
scheme_count: 1
schemes:
- authorize_url: https://mcp.divinci.app/authorize
  evidence: Send the access token in the `Authorization` header only.
  flows:
  - authorization_code
  how_to_obtain: POST https://mcp.divinci.app/register (dynamic client registration) then run the authorization code flow with PKCE (S256) to obtain an access token via the token endpoint https://mcp.divinci.app/token. Refresh tokens are issued when the offline_access scope is requested. Tokens may be revoked at https://mcp.divinci.app/revoke.
  name: oauth2_dynamic_client_registration
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - rag:read
  - rag:write
  - chat:read
  - chat:write
  - release:read
  - release:write
  - config:read
  - config:write
  type: oauth2
slug: divinci-app-authentication
source_filename: divinci-app-authentication.yml
source_heading: Authentication Profile
source_url: https://divinci.ai/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://divinci.ai/auth.md\nsources:\n- https://divinci.ai/auth.md\ndescription: Divinci agents authenticate using OAuth 2.1 with dynamic client registration and the authorization code flow (PKCE). The access token\n  is sent in the Authorization header as a Bearer token.\nschemes:\n- type: oauth2\n  name: oauth2_dynamic_client_registration\n  evidence: Send the access token in the `Authorization` header only.\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.divinci.app/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - rag:read\n  - rag:write\n  - chat:read\n  - chat:write\n  - release:read\n  - release:write\n  - config:read\n  - config:write\n  how_to_obtain: POST https://mcp.divinci.app/register (dynamic client registration) then run the authorization code flow with PKCE (S256) to\n    obtain an access token via the token endpoint\
  \ https://mcp.divinci.app/token. Refresh tokens are issued when the offline_access scope is requested.\n    Tokens may be revoked at https://mcp.divinci.app/revoke.\nnote: Credentials are passed only in the HTTP Authorization header as `Bearer <token>`; query‑string credentials are rejected.\ndocs: https://divinci.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/divinci-app/authentication/divinci-app-authentication.yml
summary_line: 1 scheme
tags:
- Website Integration
- Conversational AI
- No-Code
- Customer Service
- phone integration
---
