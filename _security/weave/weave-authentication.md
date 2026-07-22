---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Weave Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- refreshToken
overview: Weave secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, and refreshToken flow(s).
provider_name: Weave
provider_slug: weave
scheme_count: 1
schemes:
- authorization_endpoint: https://oidc.weaveconnect.com/oauth2/auth
  code_challenge_methods:
  - S256
  - plain
  end_session_endpoint: https://oidc.weaveconnect.com/oauth2/sessions/logout
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://oidc.weaveconnect.com
  jwks_uri: https://oidc.weaveconnect.com/.well-known/jwks.json
  name: WeaveOIDC
  openIdConnectUrl: https://oidc.weaveconnect.com/.well-known/openid-configuration
  revocation_endpoint: https://oidc.weaveconnect.com/oauth2/revoke
  sources:
  - well-known/weave-openid-configuration.json
  token_endpoint: https://oidc.weaveconnect.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://oidc.weaveconnect.com/userinfo
slug: weave-authentication
source_filename: weave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://oidc.weaveconnect.com/.well-known/openid-configuration\ndocs: https://dp.getweave.com/docs\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - refreshToken\n  pkce: S256\nschemes:\n- name: WeaveOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://oidc.weaveconnect.com/.well-known/openid-configuration\n  issuer: https://oidc.weaveconnect.com\n  authorization_endpoint: https://oidc.weaveconnect.com/oauth2/auth\n  token_endpoint: https://oidc.weaveconnect.com/oauth2/token\n  userinfo_endpoint: https://oidc.weaveconnect.com/userinfo\n  jwks_uri: https://oidc.weaveconnect.com/.well-known/jwks.json\n  revocation_endpoint: https://oidc.weaveconnect.com/oauth2/revoke\n  end_session_endpoint: https://oidc.weaveconnect.com/oauth2/sessions/logout\n  grant_types:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n\
  \  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  code_challenge_methods:\n  - S256\n  - plain\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/weave-openid-configuration.json\nnotes: >-\n  Weave's developer platform authorizes API calls to api.weaveconnect.com with\n  OAuth 2.0 / OpenID Connect bearer tokens issued by an Ory Hydra authorization\n  server at oidc.weaveconnect.com. Partner apps use the authorization_code flow\n  (with PKCE S256) for user-context access and client_credentials for\n  service-to-service access. No public OpenAPI is published, so this profile is\n  derived from the live OIDC discovery document rather than spec securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/authentication/weave-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Communication
- Messaging
- Payments
- Healthcare
- VoIP
- Telephony
- Reviews
- Scheduling
- SMB
- Developer Platform
- OAuth
---
