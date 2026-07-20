---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Eagle Eye Networks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
overview: Eagle Eye Networks secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and deviceCode flow(s).
provider_name: Eagle Eye Networks
provider_slug: eagle-eye-networks
scheme_count: 2
schemes:
- endpoints:
    end_session: https://auth.eagleeyenetworks.com/connect/logout
    introspection: https://auth.eagleeyenetworks.com/oauth2/introspect
    jwks: https://auth.eagleeyenetworks.com/oauth2/jwks
    revocation: https://auth.eagleeyenetworks.com/oauth2/revoke
    userinfo: https://auth.eagleeyenetworks.com/oauth2/userinfo
  flows:
  - authorizationUrl: https://auth.eagleeyenetworks.com/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://auth.eagleeyenetworks.com/oauth2/token
    scopes:
      vms.all: Full access to the Eagle Eye Video API Platform
    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token
  - flow: clientCredentials
    scopes:
      vms.all: Full access to the Eagle Eye Video API Platform
    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token
  - deviceAuthorizationUrl: https://auth.eagleeyenetworks.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token
  issuer: https://auth.eagleeyenetworks.com
  name: OAuth2
  sources:
  - well-known/eagle-eye-networks-openid-configuration.json
  type: oauth2
- name: OpenIDConnect
  openIdConnectUrl: https://auth.eagleeyenetworks.com/.well-known/openid-configuration
  scopes:
  - openid
  - profile
  - email
  sources:
  - well-known/eagle-eye-networks-openid-configuration.json
  type: openIdConnect
slug: eagle-eye-networks-authentication
source_filename: eagle-eye-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.eagleeyenetworks.com/.well-known/openid-configuration\ndocs: https://developer.eagleeyenetworks.com/docs/auth\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - deviceCode\n  token_transport: Authorization header, Bearer <access_token>\n  pkce: S256\n  confidential_client: true\n  client_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://auth.eagleeyenetworks.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eagleeyenetworks.com/oauth2/authorize\n    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token\n    refreshUrl: https://auth.eagleeyenetworks.com/oauth2/token\n    scopes:\n      vms.all: Full access to the Eagle Eye Video\
  \ API Platform\n  - flow: clientCredentials\n    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token\n    scopes:\n      vms.all: Full access to the Eagle Eye Video API Platform\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.eagleeyenetworks.com/oauth2/device_authorization\n    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token\n  endpoints:\n    userinfo: https://auth.eagleeyenetworks.com/oauth2/userinfo\n    jwks: https://auth.eagleeyenetworks.com/oauth2/jwks\n    introspection: https://auth.eagleeyenetworks.com/oauth2/introspect\n    revocation: https://auth.eagleeyenetworks.com/oauth2/revoke\n    end_session: https://auth.eagleeyenetworks.com/connect/logout\n  sources:\n  - well-known/eagle-eye-networks-openid-configuration.json\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.eagleeyenetworks.com/.well-known/openid-configuration\n  scopes:\n  - openid\n  - profile\n  - email\n  sources:\n  - well-known/eagle-eye-networks-openid-configuration.json\n\
  notes: >-\n  Access tokens are obtained from the Eagle Eye OAuth 2.0 / OIDC server and passed\n  as a Bearer token. The token response also returns a per-account httpsBaseUrl\n  (e.g. api.cNNN.eagleeyenetworks.com) that clients must use as the API host for\n  subsequent calls. Confidential clients exchange the authorization code at the\n  token endpoint using HTTP Basic (client_id:client_secret).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagle-eye-networks/refs/heads/main/authentication/eagle-eye-networks-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Security
- Video Surveillance
- Video Management
- Cloud Video
- Cameras
- Physical Security
- Video Analytics
- License Plate Recognition
- Streaming
- Webhooks
- OAuth
---
