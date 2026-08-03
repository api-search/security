---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Anvilogic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Anvilogic secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Anvilogic
provider_slug: anvilogic
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://secure.anvilogic.com/login/sso
    flow: authorizationCode
    scopes: {}
    tokenUrl: https://secure.anvilogic.com/api/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://secure.anvilogic.com/api/authentication/oauth/introspect
  issuer: https://secure.anvilogic.com
  name: AnvilogicOAuth2
  response_types_supported:
  - code
  source: https://secure.anvilogic.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://secure.anvilogic.com/mcp
  name: AnvilogicMCPBearer
  realm: mcp
  resource_metadata: https://secure.anvilogic.com/.well-known/oauth-protected-resource
  scheme: bearer
  source: https://secure.anvilogic.com/mcp (WWW-Authenticate challenge)
  type: http
slug: anvilogic-authentication
source_filename: anvilogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://secure.anvilogic.com/.well-known/oauth-authorization-server\ndocs: https://public-docs.anvilogic.com/get-started/onboarding-guide/additional-tasks\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  pkce_methods:\n  - S256\n  api_key_in: []\n  openid_connect: false\n  note: >-\n    Derived from the provider's own RFC 8414 authorization-server metadata rather\n    than from an OpenAPI document — Anvilogic publishes no public OpenAPI, and its\n    product documentation is behind the platform login.\nschemes:\n- name: AnvilogicOAuth2\n  type: oauth2\n  source: https://secure.anvilogic.com/.well-known/oauth-authorization-server\n  issuer: https://secure.anvilogic.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.anvilogic.com/login/sso\n    tokenUrl: https://secure.anvilogic.com/api/authentication/oauth/token\n    scopes: {}\n  introspection_endpoint: https://secure.anvilogic.com/api/authentication/oauth/introspect\n\
  \  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n- name: AnvilogicMCPBearer\n  type: http\n  scheme: bearer\n  source: 'https://secure.anvilogic.com/mcp (WWW-Authenticate challenge)'\n  realm: mcp\n  resource_metadata: https://secure.anvilogic.com/.well-known/oauth-protected-resource\n  applies_to:\n  - https://secure.anvilogic.com/mcp\nscopes_published: false\nscopes_note: >-\n  The authorization-server metadata declares no scopes_supported and no scope\n  reference page is published outside the customer portal, so no scopes/ artifact\n  is emitted rather than inventing one.\nplatform_authentication:\n  sso: true\n  sso_endpoint: https://secure.anvilogic.com/login/sso\n  password_login: https://secure.anvilogic.com/login\n  mfa: true\n  mfa_source: https://trust.anvilogic.com/\n  rbac: true\n  admin_docs: https://public-docs.anvilogic.com/get-started/onboarding-guide/additional-tasks\n\
  x-evidence:\n- fetched: '2026-07-31'\n  url: https://secure.anvilogic.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-07-31'\n  url: https://secure.anvilogic.com/mcp\n  http_status: 401\n  www_authenticate: 'Bearer realm=\"mcp\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anvilogic/refs/heads/main/authentication/anvilogic-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Security Operations
- Detection Engineering
- SIEM
- Threat Detection
- Artificial Intelligence
- Agents
- Model Context Protocol
- Data Lake
---
