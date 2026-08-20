---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Cerapedics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cerapedics secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cerapedics
provider_slug: cerapedics
scheme_count: 1
schemes:
- applies_to: https://mcp.cerapedics.com/mcp
  flows:
  - authorizationUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    refreshSupported: true
    scopes:
      https://mcp.cerapedics.com/mcp/user_impersonation: Act on the signed-in user's behalf against the Cerapedics MCP server
      offline_access: Issue a refresh token
      openid: OpenID Connect sign-in
      profile: Basic profile claims
    tokenUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token
  issuer: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/v2.0
  name: mcp_oauth2
  response_types_supported:
  - code
  sources:
  - well-known/cerapedics-oauth-protected-resource.json
  - well-known/cerapedics-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: cerapedics-authentication
source_filename: cerapedics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://mcp.cerapedics.com/.well-known/oauth-protected-resource\nnote: >-\n  Derived from live OAuth discovery documents rather than from an OpenAPI\n  securitySchemes block — Cerapedics publishes no OpenAPI definition. The\n  0-working/derive-authentication.py path was not applicable (no openapi/ directory).\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  bearer_methods_supported: [header]\n  identity_provider: Microsoft Entra ID\n  public_signup: false\nschemes:\n- name: mcp_oauth2\n  type: oauth2\n  applies_to: https://mcp.cerapedics.com/mcp\n  sources:\n  - well-known/cerapedics-oauth-protected-resource.json\n  - well-known/cerapedics-oauth-authorization-server.json\n  issuer: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/v2.0\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token\n    refreshSupported: true\n    code_challenge_methods_supported: [S256]\n    scopes:\n      https://mcp.cerapedics.com/mcp/user_impersonation: Act on the signed-in user's\n        behalf against the Cerapedics MCP server\n      openid: OpenID Connect sign-in\n      profile: Basic profile claims\n      offline_access: Issue a refresh token\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  response_types_supported: [code]\nchallenge:\n  status: 401\n  header: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.cerapedics.com/.well-known/oauth-protected-resource\"'\n  spec: RFC 6750 + RFC 9728\n  body: '{\"error\":\"unauthorized\",\"error_description\":\"missing or invalid bearer token\"}'\naccess:\n  self_service_signup: false\n  note: >-\n    No public developer registration exists. Tokens are issued by the Cerapedics\n    Microsoft Entra ID\
  \ tenant, so access is limited to identities in (or federated\n    into) that tenant. There is no documented partner or public onboarding path.\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - {url: 'https://mcp.cerapedics.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://mcp.cerapedics.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.cerapedics.com/mcp', http_status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerapedics/refs/heads/main/authentication/cerapedics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Medical Devices
- Orthopedics
- Orthobiologics
- Bone Graft
- Spine Surgery
- Healthcare
- Life Sciences
- MCP
---
