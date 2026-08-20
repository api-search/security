---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ccc Intelligent Solutions Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
- deviceCode
- refreshToken
overview: CCC Intelligent Solutions secures its APIs with oauth2 and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: CCC Intelligent Solutions
provider_slug: ccc-intelligent-solutions
scheme_count: 4
schemes:
- evidence: 'www-authenticate: Bearer realm="null",error="invalid_token",

    error_description="oauth.v2.InvalidAccessToken: Invalid access token"

    '
  gateway: Apigee (oauth.v2.* / keymanagement.service.* fault codes) behind Cloudflare
  in: header
  name: CCCGatewayBearer
  parameter: Authorization
  scheme: Bearer
  source: probed https://api.cccis.com/v1 (HTTP 401)
  token_issuance: not public
  type: oauth2
- code_challenge_methods:
  - S256
  dpop_signing_alg_values:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://auth.cccis.com/oauth2/v1/authorize
    device_authorization: https://auth.cccis.com/oauth2/v1/device/authorize
    end_session: https://auth.cccis.com/oauth2/v1/logout
    introspection: https://auth.cccis.com/oauth2/v1/introspect
    jwks: https://auth.cccis.com/oauth2/v1/keys
    registration: https://auth.cccis.com/oauth2/v1/clients
    revocation: https://auth.cccis.com/oauth2/v1/revoke
    token: https://auth.cccis.com/oauth2/v1/token
    userinfo: https://auth.cccis.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://auth.cccis.com
  name: CCCOktaOrgAuthorizationServer
  openIdConnectUrl: https://auth.cccis.com/.well-known/openid-configuration
  request_parameter_supported: true
  source: well-known/ccc-intelligent-solutions-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- code_challenge_methods:
  - S256
  endpoints:
    authorization: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/authorize
    introspection: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/introspect
    revocation: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/revoke
    token: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/token
    userinfo: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7
  name: CCCOktaConnectAuthorizationServer
  observed_flow: authorization_code + PKCE, scope "openid email profile connect:portal"
  openIdConnectUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/.well-known/openid-configuration
  source: well-known/ccc-intelligent-solutions-connect-openid-configuration.json
  type: openIdConnect
  used_by: https://connect.cccis.com/ (CCC Connect customer/partner portal)
- flow: clientCredentials
  name: CCCOktaClientCredentials
  note: 'client_credentials appears in grant_types_supported at the org authorization

    server (RFC 8414 metadata) only. No public/dynamic client registration is

    offered to third parties; an unauthenticated POST to the token endpoint

    returns Okta errorCode "invalid_client".

    '
  source: well-known/ccc-intelligent-solutions-oauth-authorization-server.json
  type: oauth2
slug: ccc-intelligent-solutions-authentication
source_filename: ccc-intelligent-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cccis.com/.well-known/openid-configuration\ndocs: https://www.cccsecureshare.com/Developers\nnote: |\n  Derived from live, anonymously readable discovery documents plus the live\n  OAuth challenge on the production gateway - not from an OpenAPI, because CCC\n  publishes none. There is no self-serve credential path: api.cccis.com issues\n  no public token endpoint of its own, and CCC Secure Share credentials are\n  released only after app registration, CCC review and active CIECA membership.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, password, clientCredentials, deviceCode, refreshToken]\n  public_client_registration: false\n  self_serve: false\n  gating: app registration + CCC approval + active CIECA membership (Secure Share)\nschemes:\n- name: CCCGatewayBearer\n  type: oauth2\n  in: header\n  parameter: Authorization\n  scheme: Bearer\n  source:\
  \ probed https://api.cccis.com/v1 (HTTP 401)\n  evidence: |\n    www-authenticate: Bearer realm=\"null\",error=\"invalid_token\",\n    error_description=\"oauth.v2.InvalidAccessToken: Invalid access token\"\n  gateway: Apigee (oauth.v2.* / keymanagement.service.* fault codes) behind Cloudflare\n  token_issuance: not public\n- name: CCCOktaOrgAuthorizationServer\n  type: openIdConnect\n  openIdConnectUrl: https://auth.cccis.com/.well-known/openid-configuration\n  source: well-known/ccc-intelligent-solutions-openid-configuration.json\n  issuer: https://auth.cccis.com\n  endpoints:\n    authorization: https://auth.cccis.com/oauth2/v1/authorize\n    token: https://auth.cccis.com/oauth2/v1/token\n    userinfo: https://auth.cccis.com/oauth2/v1/userinfo\n    introspection: https://auth.cccis.com/oauth2/v1/introspect\n    revocation: https://auth.cccis.com/oauth2/v1/revoke\n    registration: https://auth.cccis.com/oauth2/v1/clients\n    end_session: https://auth.cccis.com/oauth2/v1/logout\n  \
  \  device_authorization: https://auth.cccis.com/oauth2/v1/device/authorize\n    jwks: https://auth.cccis.com/oauth2/v1/keys\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  code_challenge_methods: [S256]\n  dpop_signing_alg_values: [RS256, RS384, RS512, ES256, ES384, ES512]\n  request_parameter_supported: true\n- name: CCCOktaConnectAuthorizationServer\n  type: openIdConnect\n  openIdConnectUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/.well-known/openid-configuration\n  source: well-known/ccc-intelligent-solutions-connect-openid-configuration.json\n  issuer: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7\n  used_by: https://connect.cccis.com/ (CCC Connect customer/partner portal)\n  endpoints:\n    authorization: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/authorize\n    token:\
  \ https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/token\n    userinfo: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/userinfo\n    introspection: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/introspect\n    revocation: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/revoke\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  code_challenge_methods: [S256]\n  observed_flow: authorization_code + PKCE, scope \"openid email profile connect:portal\"\n- name: CCCOktaClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  source: well-known/ccc-intelligent-solutions-oauth-authorization-server.json\n  note: |\n    client_credentials appears in grant_types_supported at the org authorization\n    server (RFC 8414 metadata) only. No public/dynamic client registration is\n    offered to third parties; an unauthenticated POST to the token endpoint\n    returns Okta errorCode \"invalid_client\"\
  .\ngaps:\n- No API key / basic-auth scheme is documented or observed anywhere.\n- 'No public developer credential flow: token issuance for api.cccis.com is\n  contract-gated, and Secure Share app credentials require CIECA membership.'\n- No mutualTLS or client-certificate requirement is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccc-intelligent-solutions/refs/heads/main/authentication/ccc-intelligent-solutions-authentication.yml
summary_line: oauth2/openIdConnect · 4 schemes
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Auto Physical Damage
- Collision Repair
- Insurtech
- Claims Technology
- CIECA
- Partner Gated
- Authentication
- OpenID Connect
---
