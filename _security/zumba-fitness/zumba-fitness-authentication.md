---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Zumba Fitness Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zumba Fitness declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zumba Fitness
provider_slug: zumba-fitness
scheme_count: 2
schemes:
- issuer: https://www.zumba.com
  name: zumba_oidc
  openIdConnectUrl: https://www.zumba.com/.well-known/openid-configuration
  type: openIdConnect
- flows:
  - authorizationUrl: https://www.zumba.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://www.zumba.com/oauth/access_token
    scopes:
      email: Access the user's email address and email_verified claim
      openid: Authenticate the end user and issue an ID token
      profile: Access basic profile claims (given_name, family_name)
    tokenUrl: https://www.zumba.com/oauth/access_token
  name: zumba_oauth2
  type: oauth2
slug: zumba-fitness-authentication
source_filename: zumba-fitness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.zumba.com/.well-known/openid-configuration (live)\nsummary: >-\n  Zumba operates an OpenID Connect 1.0 / OAuth 2.0 authorization server at\n  https://www.zumba.com. Consumer sign-in is delegated via the authorization_code\n  grant with PKCE (S256). ID tokens are signed RS256 against the published JWKS.\nschemes:\n- type: openIdConnect\n  name: zumba_oidc\n  issuer: https://www.zumba.com\n  openIdConnectUrl: https://www.zumba.com/.well-known/openid-configuration\n- type: oauth2\n  name: zumba_oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.zumba.com/oauth/authorize\n    tokenUrl: https://www.zumba.com/oauth/access_token\n    refreshUrl: https://www.zumba.com/oauth/access_token\n    scopes:\n      openid: Authenticate the end user and issue an ID token\n      email: Access the user's email address and email_verified claim\n      profile: Access basic profile claims (given_name, family_name)\n\
  endpoints:\n  authorization: https://www.zumba.com/oauth/authorize\n  token: https://www.zumba.com/oauth/access_token\n  userinfo: https://www.zumba.com/oauth/userinfo\n  jwks: https://www.zumba.com/.well-known/jwks.json\n  end_session: https://www.zumba.com/oauth/logout\ngrant_types_supported:\n- authorization_code\n- refresh_token\nresponse_types_supported:\n- code\npkce:\n  supported: true\n  code_challenge_methods:\n  - S256\ntoken_endpoint_auth_methods_supported:\n- client_secret_post\n- client_secret_basic\nid_token_signing_alg_values_supported:\n- RS256\nsubject_types_supported:\n- public\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zumba-fitness/refs/heads/main/authentication/zumba-fitness-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
