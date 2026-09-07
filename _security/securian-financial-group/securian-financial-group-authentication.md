---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Securian Financial Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Securian Financial Group declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Securian Financial Group
provider_slug: securian-financial-group
scheme_count: 2
schemes:
- description: OpenID Connect 1.0 provider. userinfo at /idp/userinfo.openid, back-channel and front-channel logout both supported.
  id: openIdConnect
  openIdConnectUrl: https://sso.securian.com/.well-known/openid-configuration
  type: openIdConnect
  verified: probed
- description: OAuth 2.0 authorization server, RFC 8414 metadata published.
  flows:
    authorizationCode:
      authorizationUrl: https://sso.securian.com/as/authorization.oauth2
      refreshUrl: https://sso.securian.com/as/token.oauth2
      tokenUrl: https://sso.securian.com/as/token.oauth2
    clientCredentials:
      tokenUrl: https://sso.securian.com/as/token.oauth2
    deviceCode:
      deviceAuthorizationUrl: https://sso.securian.com/as/device_authz.oauth2
      tokenUrl: https://sso.securian.com/as/token.oauth2
    implicit:
      authorizationUrl: https://sso.securian.com/as/authorization.oauth2
    password:
      tokenUrl: https://sso.securian.com/as/token.oauth2
  id: oauth2
  type: oauth2
  verified: probed
slug: securian-financial-group-authentication
source_filename: securian-financial-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://sso.securian.com/.well-known/openid-configuration\nnote: >-\n  Derived entirely from Securian's own published discovery documents — there is no public\n  OpenAPI to read securitySchemes from, and no public developer authentication page.\n  Everything below is read verbatim out of the OpenID Connect discovery document and the\n  RFC 8414 authorization-server metadata document saved in well-known/.\nprovider: Securian Financial Group\nissuer: https://sso.securian.com\nplatform: PingFederate (Ping Identity) — inferred from the ping_* endpoints in the discovery document\nschemes:\n  - id: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://sso.securian.com/.well-known/openid-configuration\n    description: >-\n      OpenID Connect 1.0 provider. userinfo at /idp/userinfo.openid, back-channel and\n      front-channel logout both supported.\n    verified: probed\n  - id: oauth2\n    type: oauth2\n    description:\
  \ OAuth 2.0 authorization server, RFC 8414 metadata published.\n    verified: probed\n    flows:\n      authorizationCode:\n        authorizationUrl: https://sso.securian.com/as/authorization.oauth2\n        tokenUrl: https://sso.securian.com/as/token.oauth2\n        refreshUrl: https://sso.securian.com/as/token.oauth2\n      clientCredentials:\n        tokenUrl: https://sso.securian.com/as/token.oauth2\n      implicit:\n        authorizationUrl: https://sso.securian.com/as/authorization.oauth2\n      password:\n        tokenUrl: https://sso.securian.com/as/token.oauth2\n      deviceCode:\n        deviceAuthorizationUrl: https://sso.securian.com/as/device_authz.oauth2\n        tokenUrl: https://sso.securian.com/as/token.oauth2\nendpoints:\n  authorization: https://sso.securian.com/as/authorization.oauth2\n  token: https://sso.securian.com/as/token.oauth2\n  pushed_authorization_request: https://sso.securian.com/as/par.oauth2\n  device_authorization: https://sso.securian.com/as/device_authz.oauth2\n\
  \  introspection: https://sso.securian.com/as/introspect.oauth2\n  revocation: https://sso.securian.com/as/revoke_token.oauth2\n  userinfo: https://sso.securian.com/idp/userinfo.openid\n  registration: https://sso.securian.com/as/clients.oauth2\n  end_session: https://sso.securian.com/idp/init_logout.openid\n  jwks: https://sso.securian.com/pf/JWKS\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:openid:params:grant-type:ciba\n  - urn:pingidentity.com:oauth2:grant_type:validate_bearer\nclient_authentication_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - none\npkce:\n  supported: true\n  code_challenge_methods: [S256]\nsender_constrained_tokens:\n\
  \  dpop:\n    supported: true\n    signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512, PS256, PS384, PS512]\n  mtls_client_auth: true\n  mtls_certificate_bound_access_tokens: false\nrequest_objects:\n  request_parameter_supported: true\n  request_uri_parameter_supported: false\n  signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512, PS256, PS384, PS512]\nsubject_types_supported: [public, pairwise]\nclaims_supported: [sub]\ngaps:\n  - >-\n    No public developer authentication documentation. Securian's product APIs\n    (Securian Platform Connect, FlexTech, LifeBenefits) are onboarded through a sales or\n    partner agreement, so how a partner obtains a client_id for this authorization server\n    is not published anywhere we could fetch.\n  - >-\n    claims_supported lists only \"sub\" — an unusually thin claim set for an OIDC provider,\n    which typically means claims are configured per relying party rather than advertised.\n  - authorization_response_iss_parameter_supported\
  \ is false (RFC 9207 not enabled).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securian-financial-group/refs/heads/main/authentication/securian-financial-group-authentication.yml
summary_line: 2 schemes
tags:
- Fortune 1000
- Financial Services
- Insurance
- Life Insurance
- Annuities
- Retirement
- Group Benefits
- Employee Benefits
---
