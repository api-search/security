---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Zspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: zSpace declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: zSpace
provider_slug: zspace
scheme_count: 3
schemes:
- description: OpenID Connect via Keycloak. Bearer access tokens are issued from the realm token endpoint and validated against the published JWKS.
  id: openIdConnect
  in: header
  openIdConnectUrl: https://auth.zspace.com/auth/realms/master/.well-known/openid-configuration
  scheme: bearer
  type: openIdConnect
- flows:
    authorizationCode:
      authorizationUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth
      refreshUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token
      scopes_ref: scopes/zspace-scopes.yml
      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token
    clientCredentials:
      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token
    deviceCode:
      deviceAuthorizationUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth/device
    password:
      note: Resource-owner password grant is advertised in grant_types_supported. Recorded as published, not recommended.
      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token
  id: oauth2
  type: oauth2
- description: The developer portal API itself is cookie-session based. An unauthenticated GET https://api.zspace.com/v2/auth/sig returns {"status":"auth-error","loggedin":"false","msg":"Missing cookie"} (HTTP 200), and GET https://api.zspace.com/v2/social/get_csrf issues a CSRF token ({"csrf":"..."}) for the login flow.
  id: session_cookie
  in: cookie
  observed:
  - status: 200
    url: https://api.zspace.com/v2/auth/sig
  - status: 200
    url: https://api.zspace.com/v2/social/get_csrf
  type: apiKey
slug: zspace-authentication
source_filename: zspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://auth.zspace.com/auth/realms/master/.well-known/openid-configuration\nnote: >-\n  Derived from the production Keycloak OpenID Connect discovery document, fetched\n  anonymously. No OpenAPI securitySchemes block exists to derive from — the zSpace\n  developer API publishes no public contract — so this profile records the identity\n  provider's own machine-readable metadata plus the auth behaviour observed on live\n  unauthenticated calls to https://api.zspace.com/v2.\nprovider:\n  type: keycloak\n  issuer: https://auth.zspace.com/auth/realms/master\n  realm: master\n  discovery: https://auth.zspace.com/auth/realms/master/.well-known/openid-configuration\n  jwks_uri: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/certs\n  non_production_realm:\n    issuer: https://auth.devqastage.zspace.com/auth/realms/master\n    note: >-\n      The live production redirect from https://api.zspace.com/v2/api/docs sends\
  \ the user\n      to auth.devqastage.zspace.com with client_id=tester, not to auth.zspace.com. Recorded\n      as observed; both realms answer their discovery document anonymously.\nschemes:\n- id: openIdConnect\n  type: openIdConnect\n  in: header\n  scheme: bearer\n  openIdConnectUrl: https://auth.zspace.com/auth/realms/master/.well-known/openid-configuration\n  description: >-\n    OpenID Connect via Keycloak. Bearer access tokens are issued from the realm token\n    endpoint and validated against the published JWKS.\n- id: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth\n      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token\n      refreshUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token\n      scopes_ref: scopes/zspace-scopes.yml\n    clientCredentials:\n      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token\n\
  \    deviceCode:\n      deviceAuthorizationUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth/device\n    password:\n      tokenUrl: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token\n      note: >-\n        Resource-owner password grant is advertised in grant_types_supported. Recorded as\n        published, not recommended.\n- id: session_cookie\n  type: apiKey\n  in: cookie\n  description: >-\n    The developer portal API itself is cookie-session based. An unauthenticated\n    GET https://api.zspace.com/v2/auth/sig returns\n    {\"status\":\"auth-error\",\"loggedin\":\"false\",\"msg\":\"Missing cookie\"} (HTTP 200),\n    and GET https://api.zspace.com/v2/social/get_csrf issues a CSRF token\n    ({\"csrf\":\"...\"}) for the login flow.\n  observed:\n  - url: https://api.zspace.com/v2/auth/sig\n    status: 200\n  - url: https://api.zspace.com/v2/social/get_csrf\n    status: 200\nendpoints:\n  authorization: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth\n\
  \  token: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token\n  userinfo: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/userinfo\n  introspection: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/token/introspect\n  revocation: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/revoke\n  end_session: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/logout\n  registration: https://auth.zspace.com/auth/realms/master/clients-registrations/openid-connect\n  pushed_authorization_request: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/ext/par/request\n  device_authorization: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/auth/device\n  backchannel_authentication: https://auth.zspace.com/auth/realms/master/protocol/openid-connect/ext/ciba/auth\ngrant_types_supported:\n- authorization_code\n- implicit\n- refresh_token\n- password\n- client_credentials\n- urn:ietf:params:oauth:grant-type:device_code\n\
  - urn:openid:params:grant-type:ciba\ntoken_endpoint_auth_methods_supported:\n- private_key_jwt\n- client_secret_basic\n- client_secret_post\n- tls_client_auth\n- client_secret_jwt\ncode_challenge_methods_supported:\n- plain\n- S256\nclaims_supported:\n- aud\n- sub\n- iss\n- auth_time\n- name\n- given_name\n- family_name\n- preferred_username\n- email\n- acr\nmutual_tls:\n  supported: true\n  evidence: >-\n    tls_client_auth in token_endpoint_auth_methods_supported and\n    tls_client_certificate_bound_access_tokens in the discovery document.\ngaps:\n- >-\n  No public API reference documents this authentication model. The Swagger UI at\n  https://api.zspace.com/v2/api/docs exists but 302s into the Keycloak authorization\n  endpoint, so an integrator cannot read the contract the tokens are for.\n- No security.txt, no documented API key programme, no public token-issuance instructions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zspace/refs/heads/main/authentication/zspace-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Education
- Augmented Reality
- Virtual Reality
- EdTech
- Hardware
- 3D
- Simulation
- Career and Technical Education
- Developer SDK
---
