---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Coteach Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CoTeach secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CoTeach
provider_slug: coteach
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://www.coteach.ai/api/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://www.coteach.ai/api/oauth/register
    scopes:
    - openid
    - email
    - profile
    - offline_access
    tokenUrl: https://www.coteach.ai/api/oauth/token
    token_endpoint_auth_methods:
    - none
  name: OAuth2
  sources:
  - https://www.coteach.ai/.well-known/oauth-authorization-server
  type: oauth2
- issuer: https://www.coteach.ai
  name: OpenIDConnect
  openIdConnectUrl: https://www.coteach.ai/.well-known/openid-configuration
  sources:
  - https://www.coteach.ai/.well-known/openid-configuration
  type: openIdConnect
slug: coteach-authentication
source_filename: coteach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.coteach.ai/.well-known/oauth-authorization-server\ndocs: https://www.coteach.ai/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  public_client: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.coteach.ai/api/oauth/authorize\n    tokenUrl: https://www.coteach.ai/api/oauth/token\n    registrationUrl: https://www.coteach.ai/api/oauth/register\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - none\n    scopes:\n    - openid\n    - email\n    - profile\n    - offline_access\n  sources:\n  - https://www.coteach.ai/.well-known/oauth-authorization-server\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.coteach.ai/.well-known/openid-configuration\n\
  \  issuer: https://www.coteach.ai\n  sources:\n  - https://www.coteach.ai/.well-known/openid-configuration\nnotes: Derived from CoTeach's published OIDC discovery and RFC 8414 authorization-server\n  metadata. Public-client authorization-code flow with PKCE (S256) and RFC 7591\n  dynamic client registration; this is the auth surface protecting the hosted MCP\n  server. No OpenAPI is published, so this profile is sourced entirely from the\n  live .well-known documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coteach/refs/heads/main/authentication/coteach-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Education
- EdTech
- Mathematics
- K-12
- Teachers
- Curriculum
- Lesson Planning
- AI Assistant
- Illustrative Mathematics
- MCP
---
