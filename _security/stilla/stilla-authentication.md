---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Stilla Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Stilla secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Stilla
provider_slug: stilla
scheme_count: 2
schemes:
- authorization_endpoint: https://login.stilla.ai/oauth2/authorize
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  device_authorization_endpoint: https://login.stilla.ai/oauth2/device_authorization
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://login.stilla.ai/oauth2/introspection
  issuer: https://login.stilla.ai
  jwks_uri: https://login.stilla.ai/oauth2/jwks
  name: OAuth2
  registration_endpoint: https://login.stilla.ai/oauth2/register
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://login.stilla.ai/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- name: OpenIDConnect
  openIdConnectUrl: https://login.stilla.ai/.well-known/openid-configuration
  type: openIdConnect
slug: stilla-authentication
source_filename: stilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.stilla.ai/.well-known/oauth-authorization-server\ndocs: https://stilla.ai/docs/integrations/stilla-mcp\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\n  provider: WorkOS AuthKit (login.stilla.ai)\nschemes:\n  - name: OAuth2\n    type: oauth2\n    issuer: https://login.stilla.ai\n    authorization_endpoint: https://login.stilla.ai/oauth2/authorize\n    token_endpoint: https://login.stilla.ai/oauth2/token\n    device_authorization_endpoint: https://login.stilla.ai/oauth2/device_authorization\n    introspection_endpoint: https://login.stilla.ai/oauth2/introspection\n    jwks_uri: https://login.stilla.ai/oauth2/jwks\n    registration_endpoint: https://login.stilla.ai/oauth2/register   # RFC 7591 dynamic client registration\n    grant_types_supported: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:device_code\"]\n  \
  \  code_challenge_methods_supported: [S256]                          # PKCE required\n    token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n    client_id_metadata_document_supported: true\n    scopes_supported: [openid, profile, email, offline_access]\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.stilla.ai/.well-known/openid-configuration\nenterprise:\n  # From https://stilla.ai/security\n  sso: SAML\n  provisioning: SCIM\n  access_control: role-based permissions + full audit logs\nnotes: >-\n  The Stilla REST API (api.stilla.ai) and the MCP server are protected by OAuth 2.0 /\n  OIDC via WorkOS AuthKit. Bearer tokens are passed in the Authorization header. PKCE\n  (S256) is mandatory, and clients may register dynamically. Enterprise tenants add\n  SAML SSO and SCIM provisioning. The OpenAPI document at api.stilla.ai/openapi.json is\n  gated behind login and not publicly retrievable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stilla/refs/heads/main/authentication/stilla-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic
- Productivity
- Collaboration
- MCP
- Automation
- Developer Tools
- Enterprise
---
