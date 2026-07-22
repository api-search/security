---
api_key_in:
- header
api_specs:
- filename: openpath-openapi-original.json
  format: json
  label: Openpath API
  slug: openpath-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/openapi/openpath-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Openpath Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Openpath secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Openpath
provider_slug: openpath
scheme_count: 3
schemes:
- description: Primary auth. A JWT access token obtained from the Login API (POST /auth/login, optionally with mfa.totpCode) is sent in the Authorization header. The token carries fine-grained scope strings of the form o{orgId}-<resource>:<r|w>. Refresh via /auth/refreshLogin; validate via /auth/validateAccessToken.
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/openpath-openapi-original.json
  type: apiKey
- description: HTTP Basic Authentication is also accepted per the API docs.
  name: basic
  scheme: basic
  sources:
  - https://openpath.readme.io/docs/using-the-api
  type: http
- authorizationUrl: https://helium.prod.openpath.com/oauth/authorize
  description: An OpenID Connect / OAuth2 authorization server (issuer helium.prod.openpath.com) is advertised at /.well-known/openid-configuration, supporting authorization_code + refresh_token grants with PKCE (S256) and RS256 ID tokens.
  flow: authorizationCode
  name: oauth2-oidc
  pkce: S256
  scopes:
  - openid
  - profile
  - email
  sources:
  - well-known/openpath-openid-configuration.json
  tokenUrl: https://helium.prod.openpath.com/oauth/token
  type: oauth2
slug: openpath-authentication
source_filename: openpath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/openpath-openapi-original.json + https://openpath.readme.io/docs/using-the-api + well-known/openpath-openid-configuration.json\ndocs: https://openpath.readme.io/docs/using-the-api\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Primary auth. A JWT access token obtained from the Login API (POST /auth/login,\n    optionally with mfa.totpCode) is sent in the Authorization header. The token\n    carries fine-grained scope strings of the form o{orgId}-<resource>:<r|w>.\n    Refresh via /auth/refreshLogin; validate via /auth/validateAccessToken.\n  sources:\n  - openapi/openpath-openapi-original.json\n- name: basic\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication is also accepted per the API docs.\n  sources:\n  - https://openpath.readme.io/docs/using-the-api\n\
  - name: oauth2-oidc\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://helium.prod.openpath.com/oauth/authorize\n  tokenUrl: https://helium.prod.openpath.com/oauth/token\n  pkce: S256\n  scopes: [openid, profile, email]\n  description: >-\n    An OpenID Connect / OAuth2 authorization server (issuer helium.prod.openpath.com)\n    is advertised at /.well-known/openid-configuration, supporting authorization_code\n    + refresh_token grants with PKCE (S256) and RS256 ID tokens.\n  sources:\n  - well-known/openpath-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/authentication/openpath-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Security
- Access Control
- Physical Security
- Identity
- Credentials
- IoT
- Smart Building
- Avigilon Alta
- Motorola Solutions
---
