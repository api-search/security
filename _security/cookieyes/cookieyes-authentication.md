---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cookieyes Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cookieyes secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cookieyes
provider_slug: cookieyes
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://app.cookieyes.com/oauth2/auth
    flow: authorizationCode
    pkce_methods:
    - S256
    revocationUrl: https://app.cookieyes.com/oauth2/revoke
    scopes:
    - openid
    - offline
    - offline_access
    - mcp:read
    - mcp:write
    tokenUrl: https://app.cookieyes.com/oauth2/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://app.cookieyes.com
  name: OAuth2
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  jwks_uri: https://app.cookieyes.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://app.cookieyes.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  - pairwise
  type: openIdConnect
  userinfo_endpoint: https://app.cookieyes.com/userinfo
slug: cookieyes-authentication
source_filename: cookieyes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.cookieyes.com/.well-known/openid-configuration\ndocs: https://app.cookieyes.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://app.cookieyes.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.cookieyes.com/oauth2/auth\n    tokenUrl: https://app.cookieyes.com/oauth2/token\n    revocationUrl: https://app.cookieyes.com/oauth2/revoke\n    pkce_methods:\n    - S256\n    scopes:\n    - openid\n    - offline\n    - offline_access\n    - mcp:read\n    - mcp:write\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.cookieyes.com/.well-known/openid-configuration\n\
  \  userinfo_endpoint: https://app.cookieyes.com/userinfo\n  jwks_uri: https://app.cookieyes.com/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  - pairwise\nregistration_endpoint: https://app.cookieyes.com/oauth2/register\nnotes: >-\n  CookieYes runs a standards-compliant OAuth 2.0 / OpenID Connect provider on\n  app.cookieyes.com backing its hosted MCP server. Authorization-code flow with\n  mandatory PKCE (S256), refresh tokens, RFC 7591 dynamic client registration,\n  and RFC 8414 authorization-server metadata. Public clients may use\n  token_endpoint_auth_method \"none\". This profile is derived from the live OIDC\n  discovery document; CookieYes does not publish a separate REST OpenAPI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cookieyes/refs/heads/main/authentication/cookieyes-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consent Management
- Privacy
- GDPR
- CCPA
- Cookie Consent
- Compliance
- Data Protection
- MCP
---
