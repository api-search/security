---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 1Up Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 1up secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 1up
provider_slug: 1up
scheme_count: 2
schemes:
- applies_to: https://mcp.1up.ai/mcp
  challenge_observed:
    body: '{"error":"unauthorized","error_description":"Missing Authorization header"}'
    http_status: 401
    url: https://mcp.1up.ai/mcp
    www_authenticate: Bearer
  flows:
  - authorizationUrl: https://mcp.1up.ai/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    grant_types_supported:
    - authorization_code
    - refresh_token
    registrationUrl: https://mcp.1up.ai/register
    response_types_supported:
    - code
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://mcp.1up.ai/token
    token_endpoint_auth_methods_supported:
    - none
  issuer: https://mcp.1up.ai
  name: 1up MCP OAuth 2.1
  protected_resource:
    authorization_servers:
    - https://mcp.1up.ai
    bearer_methods_supported:
    - header
    resource: https://mcp.1up.ai/mcp
    resource_name: 1up MCP Server
  public_client_id: TAWQL8mbs0eHLzaBaxV3Va5vH6qal4Wq
  public_client_id_note: Published by the provider in both the discovery document and the copy-paste Claude Code config in their own docs. It is a public OAuth client identifier, not a secret.
  sources:
  - well-known/1up-oauth-authorization-server.json
  - well-known/1up-oauth-protected-resource.json
  type: oauth2
- applies_to: https://api.1upapi.com/api/v1/
  challenge_observed:
    body: '{"detail":"Authentication credentials were not provided."}'
    http_status: 401
    url: https://api.1upapi.com/api/v1/
  documented: false
  name: 1up platform API token
  note: Not part of a public developer program. The base URL and Authorization-header behaviour are recorded here only because 1up's own published PyPI package names them; there is no public reference, no published spec and no self-service key issuance. The host answers an anonymous GET /api/v1/ with HTTP 401 and the Django REST Framework body {"detail":"Authentication credentials were not provided."}. Tokens are Auth0-issued (audience https://1up-app.us.auth0.com/api/v2/) and obtained via `1up-mcp auth login`.
  scheme: bearer
  sources:
  - pypi:1up-mcp==0.1.0 (oneup_mcp/api_client.py
  - oneup_mcp/config.py)
  type: http
slug: 1up-authentication
source_filename: 1up-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.1up.ai/.well-known/oauth-authorization-server ;\n  https://mcp.1up.ai/.well-known/oauth-protected-resource ;\n  https://help.1up.ai/en/articles/14304740-mcp\ndocs: https://help.1up.ai/en/articles/14304740-mcp\nnote: >-\n  Derived from probed RFC 8414 / RFC 9728 discovery documents and observed 401 responses,\n  not from an OpenAPI — 1up publishes no OpenAPI. Two distinct auth surfaces exist and they\n  are not the same thing: the public MCP server (OAuth 2.1) and the platform REST host\n  api.1upapi.com (undocumented, token-authenticated, Django REST Framework).\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods: [header]\n  pkce: [S256]\n  dynamic_client_registration: true\n  identity_provider: Auth0 (1up-app.us.auth0.com)\n  human_sso: >-\n    Single Sign-On is a paid platform feature from the Starter tier upward\n    (https://help.1up.ai/en/articles/13401537-enabling-single-sign-on-sso).\n\
  schemes:\n- name: 1up MCP OAuth 2.1\n  type: oauth2\n  applies_to: https://mcp.1up.ai/mcp\n  sources: [well-known/1up-oauth-authorization-server.json, well-known/1up-oauth-protected-resource.json]\n  issuer: https://mcp.1up.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.1up.ai/authorize\n    tokenUrl: https://mcp.1up.ai/token\n    registrationUrl: https://mcp.1up.ai/register\n    code_challenge_methods_supported: [S256]\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none]\n    scopes: [openid, profile, email, offline_access]\n  public_client_id: TAWQL8mbs0eHLzaBaxV3Va5vH6qal4Wq\n  public_client_id_note: >-\n    Published by the provider in both the discovery document and the copy-paste Claude Code\n    config in their own docs. It is a public OAuth client identifier, not a secret.\n  protected_resource:\n    resource: https://mcp.1up.ai/mcp\n    authorization_servers:\
  \ [https://mcp.1up.ai]\n    bearer_methods_supported: [header]\n    resource_name: 1up MCP Server\n  challenge_observed:\n    url: https://mcp.1up.ai/mcp\n    http_status: 401\n    www_authenticate: Bearer\n    body: '{\"error\":\"unauthorized\",\"error_description\":\"Missing Authorization header\"}'\n- name: 1up platform API token\n  type: http\n  scheme: bearer\n  applies_to: https://api.1upapi.com/api/v1/\n  documented: false\n  sources: [pypi:1up-mcp==0.1.0 (oneup_mcp/api_client.py, oneup_mcp/config.py)]\n  note: >-\n    Not part of a public developer program. The base URL and Authorization-header behaviour\n    are recorded here only because 1up's own published PyPI package names them; there is no\n    public reference, no published spec and no self-service key issuance. The host answers\n    an anonymous GET /api/v1/ with HTTP 401 and the Django REST Framework body\n    {\"detail\":\"Authentication credentials were not provided.\"}. Tokens are Auth0-issued\n    (audience https://1up-app.us.auth0.com/api/v2/)\
  \ and obtained via `1up-mcp auth login`.\n  challenge_observed:\n    url: https://api.1upapi.com/api/v1/\n    http_status: 401\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1up/refs/heads/main/authentication/1up-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Knowledge Management
- RFP Automation
- Security Questionnaires
- Model Context Protocol
- Agents
- SaaS
- Revenue Operations
---
