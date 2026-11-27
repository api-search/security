---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Clueso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clueso declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clueso
provider_slug: clueso-io
scheme_count: 1
schemes:
- applies_to: https://connect.clueso.io/mcp
  authorization_endpoint: https://auth.clueso.io/oauth/2.1/authorize
  docs: https://help.clueso.io/mcp-setup
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://auth.clueso.io/oauth/2.1
  name: clueso-mcp-oauth
  pkce: S256
  registration_endpoint: https://auth.clueso.io/oauth/2.1/register
  scopes:
  - openid
  - email
  - profile
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  user_flow: The docs say a browser window opens, the user signs in to Clueso and clicks Allow to authorize the AI assistant.
slug: clueso-io-authentication
source_filename: clueso-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Clueso authentication\ngenerated: '2026-11-04'\nmethod: probed\nsource: https://connect.clueso.io/.well-known/oauth-protected-resource\ndocs: https://help.clueso.io/mcp-setup\nnote: Clueso publishes no REST API. The only programmatic surface is the remote MCP server at https://connect.clueso.io/mcp, which is protected by OAuth 2.1. Values below come from the protected-resource metadata (HTTP 200) and the authorization-server metadata at https://auth.clueso.io/.well-known/oauth-authorization-server/oauth/2.1 (HTTP 200), both fetched by GET on 2026-11-04. No token, register or authorize endpoint was called.\nschemes:\n- name: clueso-mcp-oauth\n  type: oauth2\n  applies_to: https://connect.clueso.io/mcp\n  issuer: https://auth.clueso.io/oauth/2.1\n  authorization_endpoint: https://auth.clueso.io/oauth/2.1/authorize\n  registration_endpoint: https://auth.clueso.io/oauth/2.1/register\n  dynamic_client_registration: true\n  grant_types: [authorization_code, refresh_token]\n\
  \  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  scopes: [openid, email, profile]\n  user_flow: The docs say a browser window opens, the user signs in to Clueso and clicks Allow to authorize the AI assistant.\n  docs: https://help.clueso.io/mcp-setup\n"
source_yaml_url: https://artifacts.apis.io/clueso-io/authentication/clueso-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Video
- Documentation
- Screen Recording
- Video Creation
- Knowledge Base
- Training
- MCP
---
