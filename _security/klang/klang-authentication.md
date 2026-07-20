---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Klang Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
- deviceCode
- refreshToken
overview: Klang Games secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Klang Games
provider_slug: klang
scheme_count: 2
schemes:
- issuer: https://seed.game
  name: SEEDOpenIDConnect
  openIdConnectUrl: https://seed.game/.well-known/openid-configuration
  sources:
  - well-known/klang-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://login.seed.game/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.seed.game/oauth2/token
  - authorizationUrl: https://login.seed.game/oauth2/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://login.seed.game/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://login.seed.game/oauth2/token
  - deviceAuthorizationUrl: https://login.seed.game/oauth2/device_authorize
    flow: deviceCode
    tokenUrl: https://login.seed.game/oauth2/token
  name: SEEDOAuth2
  sources:
  - well-known/klang-openid-configuration.json
  type: oauth2
slug: klang-authentication
source_filename: klang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://seed.game/.well-known/openid-configuration\ndocs: https://seed.game/login\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - password\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  api_key_in: []\n  note: >-\n    Klang publishes no developer-facing authentication documentation. This\n    profile is read verbatim from the OpenID Connect discovery documents served\n    for the SEED player account system. The endpoint shape (oauth2/authorize,\n    oauth2/device_authorize, applicationId + authenticationType claims)\n    identifies the identity provider as FusionAuth.\nschemes:\n- name: SEEDOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://seed.game/.well-known/openid-configuration\n  issuer: https://seed.game\n  sources:\n  - well-known/klang-openid-configuration.json\n- name: SEEDOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://login.seed.game/oauth2/authorize\n    tokenUrl: https://login.seed.game/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://login.seed.game/oauth2/authorize\n  - flow: password\n    tokenUrl: https://login.seed.game/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://login.seed.game/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.seed.game/oauth2/device_authorize\n    tokenUrl: https://login.seed.game/oauth2/token\n  sources:\n  - well-known/klang-openid-configuration.json\nendpoints:\n  authorization: https://login.seed.game/oauth2/authorize\n  token: https://login.seed.game/oauth2/token\n  device_authorization: https://login.seed.game/oauth2/device_authorize\n  userinfo: https://login.seed.game/oauth2/userinfo\n  end_session: https://login.seed.game/oauth2/logout\n  jwks: https://login.seed.game/.well-known/jwks.json\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\n- none\n\
  id_token_signing_alg_values:\n- ES256\n- ES384\n- ES512\n- HS256\n- HS384\n- HS512\n- RS256\n- RS384\n- RS512\nclaims_supported:\n- applicationId\n- at_hash\n- aud\n- authenticationType\n- birthdate\n- c_hash\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- iss\n- jti\n- middle_name\n- name\n- nbf\n- nonce\n- phone_number\n- phone_number_verified\n- picture\n- preferred_username\n- roles\n- sub\nobservations:\n- >-\n  The discovery document at https://login.seed.game/ reports issuer \"acme.com\",\n  the unchanged FusionAuth default placeholder, while the document at\n  https://seed.game/ reports the correct issuer https://seed.game. A relying\n  party validating the iss claim against the login host would reject tokens.\n- >-\n  Both the implicit and resource-owner-password grants remain enabled; RFC 9700\n  (OAuth 2.0 Security Best Current Practice) advises against both.\n- >-\n  Symmetric HS256/HS384/HS512 are advertised as ID-token signing algorithms\n  alongside\
  \ the asymmetric families.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klang/refs/heads/main/authentication/klang-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Gaming
- Game Development
- MMO
- Simulation
- Entertainment
- Identity
- OpenID Connect
- Berlin
---
