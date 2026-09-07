---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Cleveland Cliffs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- ciba
- refreshToken
overview: Cleveland-Cliffs secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, ciba, and refreshToken flow(s).
provider_name: Cleveland-Cliffs
provider_slug: cleveland-cliffs
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - S256
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://login.clevelandcliffs.com/oauth2/v1/authorize
    device_authorization: https://login.clevelandcliffs.com/oauth2/v1/device/authorize
    dynamic_client_registration: https://login.clevelandcliffs.com/oauth2/v1/clients
    end_session: https://login.clevelandcliffs.com/oauth2/v1/logout
    introspection: https://login.clevelandcliffs.com/oauth2/v1/introspect
    jwks: https://login.clevelandcliffs.com/oauth2/v1/keys
    pushed_authorization_request: https://login.clevelandcliffs.com/oauth2/v1/par
    revocation: https://login.clevelandcliffs.com/oauth2/v1/revoke
    token: https://login.clevelandcliffs.com/oauth2/v1/token
    userinfo: https://login.clevelandcliffs.com/oauth2/v1/userinfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.clevelandcliffs.com
  name: cleveland-cliffs-okta-oidc
  openIdConnectUrl: https://login.clevelandcliffs.com/.well-known/openid-configuration
  sources:
  - well-known/cleveland-cliffs-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- flows:
  - authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token
  - deviceAuthorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token
  - authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize
    flow: implicit
  issuer: https://login.clevelandcliffs.com
  name: cleveland-cliffs-okta-oauth2
  sources:
  - well-known/cleveland-cliffs-oauth-authorization-server.json
  type: oauth2
slug: cleveland-cliffs-authentication
source_filename: cleveland-cliffs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://login.clevelandcliffs.com/.well-known/openid-configuration\ndocs: https://www.clevelandcliffs.com/doing-business\nnote: >-\n  Cleveland-Cliffs publishes no developer API and therefore no API-key or bearer-token contract.\n  It does operate a first-party identity surface: an Okta tenant on its own vanity domain\n  login.clevelandcliffs.com, whose OIDC discovery document and RFC 8414 authorization-server\n  metadata are served anonymously and declare issuer https://login.clevelandcliffs.com. That is\n  the only machine-readable authentication contract the company publishes. It fronts the\n  employee/partner applications, not a public API. The B2B integration surface (EDI over SFTP\n  or an IBM Sterling VAN) authenticates out of band with SFTP credentials and trading-partner\n  IDs negotiated bilaterally, and the four portal applications (Outside Processors, iSupplier,\n  Customer Service Center, Vendor Inquiry) each present\
  \ their own username/password form.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, deviceCode, ciba, refreshToken]\n  public_api_auth: none-published\nschemes:\n  - name: cleveland-cliffs-okta-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://login.clevelandcliffs.com/.well-known/openid-configuration\n    issuer: https://login.clevelandcliffs.com\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n    endpoints:\n      authorization: https://login.clevelandcliffs.com/oauth2/v1/authorize\n      token: https://login.clevelandcliffs.com/oauth2/v1/token\n      userinfo: https://login.clevelandcliffs.com/oauth2/v1/userinfo\n      jwks: https://login.clevelandcliffs.com/oauth2/v1/keys\n      revocation: https://login.clevelandcliffs.com/oauth2/v1/revoke\n      introspection: https://login.clevelandcliffs.com/oauth2/v1/introspect\n      end_session: https://login.clevelandcliffs.com/oauth2/v1/logout\n\
  \      device_authorization: https://login.clevelandcliffs.com/oauth2/v1/device/authorize\n      pushed_authorization_request: https://login.clevelandcliffs.com/oauth2/v1/par\n      dynamic_client_registration: https://login.clevelandcliffs.com/oauth2/v1/clients\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    code_challenge_methods_supported: [S256]\n    dpop_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512]\n  - name: cleveland-cliffs-okta-oauth2\n    type: oauth2\n    sources: [well-known/cleveland-cliffs-oauth-authorization-server.json]\n    issuer: https://login.clevelandcliffs.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize\n        tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token\n      - flow:\
  \ clientCredentials\n        tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/device/authorize\n        tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token\n      - flow: implicit\n        authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize\nout_of_band:\n  - surface: EDI (X12 4010) for outside processors\n    transport: SFTP preferred; third-party VAN via IBM Sterling Supply Chain Business Network Hub\n    auth: SFTP credentials / trading-partner identifiers exchanged bilaterally during onboarding\n    docs: https://www.clevelandcliffs.com/doing-business/for-outside-processors\n  - surface: Outside Processors Portal\n    auth: username + password form\n    url: https://op.cliffssteel.com\n  - surface: iSupplier Portal\n    auth: username + password form\n    url: https://isupplier.cliffssteel.com\n  - surface: Customer Service Center (mill test\
  \ certificates)\n    auth: username + password form\n    url: https://cert.cliffssteel.com\n  - surface: Vendor Inquiry (AP / invoice status)\n    auth: username + password form\n    url: https://www.clevelandcliffs.us/vendor_inquiry/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleveland-cliffs/refs/heads/main/authentication/cleveland-cliffs-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Automotive
- Iron Ore
- Manufacturing
- Mining
- Steel
- Steelmaking
- Supply Chain
---
