---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Arphie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Arphie secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Arphie
provider_slug: arphie
scheme_count: 1
schemes:
- bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/authorize
    codeChallengeMethods:
    - S256
    - plain
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    idTokenSigningAlgs:
    - RS256
    - HS256
    - ES256
    issuer: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1
    jwksUri: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/.well-known/jwks.json
    registrationEndpoint: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/clients/register
    scopes:
    - openid
    - profile
    - email
    - phone
    - offline_access
    tokenEndpointAuthMethods:
    - client_secret_basic
    - client_secret_post
    - none
    tokenUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token
    userinfoUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/userinfo
  name: ArphieMCPOAuth
  resource: https://app.arphie.ai/api/mcp
  resource_name: Arphie MCP
  scopes_supported:
  - email
  source: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp
  type: oauth2
slug: arphie-authentication
source_filename: arphie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp\ndocs: https://www.arphie.ai/security\nnote: >-\n  Arphie publishes no REST OpenAPI, so there are no securitySchemes to derive from. The\n  authentication profile below is read from live, anonymous, machine-readable metadata:\n  the RFC 9728 protected-resource document the Arphie MCP server advertises in its 401\n  challenge, plus the RFC 8414 authorization-server metadata that document points at.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods: [header]\n  applies_to: Arphie MCP server (https://app.arphie.ai/api/mcp)\nschemes:\n- name: ArphieMCPOAuth\n  type: oauth2\n  source: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp\n  resource: https://app.arphie.ai/api/mcp\n  resource_name: Arphie MCP\n  bearer_methods_supported: [header]\n  scopes_supported: [email]\n  flows:\n  - flow: authorizationCode\n\
  \    issuer: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1\n    authorizationUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token\n    userinfoUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/userinfo\n    jwksUri: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/.well-known/jwks.json\n    registrationEndpoint: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/clients/register\n    grantTypes: [authorization_code, refresh_token]\n    codeChallengeMethods: [S256, plain]\n    tokenEndpointAuthMethods: [client_secret_basic, client_secret_post, none]\n    idTokenSigningAlgs: [RS256, HS256, ES256]\n    scopes: [openid, profile, email, phone, offline_access]\nend_user_authentication:\n  sso: true\n  protocols: [SAML 2.0, Google authentication]\n  identity_providers_named: [Okta, OneLogin, Microsoft Azure, ADFS]\n  rbac: true\n  rbac_note: Customer-defined user roles with read-only\
  \ or read-and-write permissions.\n  source: https://www.arphie.ai/security\ngaps:\n- No API keys, no personal access tokens, and no published authentication reference for developers.\n- >-\n  The only authenticated machine surface is the MCP server; there is no documented REST\n  API and therefore no REST auth model.\nx-evidence:\n- url: https://app.arphie.ai/api/mcp\n  http_status: 401\n- url: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp\n  http_status: 200\n- url: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://www.arphie.ai/security\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arphie/refs/heads/main/authentication/arphie-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Artificial Intelligence
- Sales Enablement
- RFP Automation
- Security Questionnaires
- Knowledge Management
- Go-To-Market
- MCP
- Agents
---
