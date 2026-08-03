---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Aescape Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- jwtBearer
overview: Aescape secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, and jwtBearer flow(s).
provider_name: Aescape
provider_slug: aescape
scheme_count: 1
schemes:
- backchannel_logout_session_supported: true
  backchannel_logout_supported: true
  claims_supported:
  - sub
  - aud
  - exp
  - iat
  - iss
  - auth_time
  - nonce
  - acr
  - amr
  - c_hash
  - at_hash
  - act
  - scopes
  - client_id
  - azp
  - preferred_username
  - name
  - family_name
  - given_name
  - locale
  - email
  - email_verified
  - phone_number
  - phone_number_verified
  code_challenge_methods:
  - S256
  endpoints:
    authorization: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize
    device_authorization: https://aescape-8ocoec.zitadel.cloud/oauth/v2/device_authorization
    end_session: https://aescape-8ocoec.zitadel.cloud/oidc/v1/end_session
    introspection: https://aescape-8ocoec.zitadel.cloud/oauth/v2/introspect
    jwks: https://aescape-8ocoec.zitadel.cloud/oauth/v2/keys
    registration: null
    revocation: https://aescape-8ocoec.zitadel.cloud/oauth/v2/revoke
    token: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token
    userinfo: https://aescape-8ocoec.zitadel.cloud/oidc/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_algs:
  - EdDSA
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  issuer: https://aescape-8ocoec.zitadel.cloud
  name: AescapeOIDC
  openIdConnectUrl: https://aescape-8ocoec.zitadel.cloud/.well-known/openid-configuration
  request_parameter_supported: true
  request_uri_parameter_supported: false
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - id_token
  - id_token token
  scopes: scopes/aescape-scopes.yml
  sources:
  - well-known/aescape-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: openIdConnect
slug: aescape-authentication
source_filename: aescape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://aescape-8ocoec.zitadel.cloud/.well-known/openid-configuration\nnote: >-\n  Aescape publishes no OpenAPI, so this profile is not derived from a spec. It is\n  read verbatim from the OpenID Connect discovery document served by Aescape's\n  production Zitadel identity tenant, which is the only anonymously reachable\n  machine-readable auth contract in the estate. The application API host\n  (api.aescape.com) and the developer documentation site (developer.aescape.com)\n  publish no auth documentation publicly; developer.aescape.com is itself gated\n  behind HTTP Basic auth.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, deviceCode, jwtBearer]\n  pkce: [S256]\n  identity_provider: Zitadel (hosted)\n  provider_managed: true\nschemes:\n- name: AescapeOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://aescape-8ocoec.zitadel.cloud/.well-known/openid-configuration\n\
  \  issuer: https://aescape-8ocoec.zitadel.cloud\n  sources: [well-known/aescape-openid-configuration.json]\n  endpoints:\n    authorization: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize\n    token: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token\n    userinfo: https://aescape-8ocoec.zitadel.cloud/oidc/v1/userinfo\n    jwks: https://aescape-8ocoec.zitadel.cloud/oauth/v2/keys\n    introspection: https://aescape-8ocoec.zitadel.cloud/oauth/v2/introspect\n    revocation: https://aescape-8ocoec.zitadel.cloud/oauth/v2/revoke\n    end_session: https://aescape-8ocoec.zitadel.cloud/oidc/v1/end_session\n    device_authorization: https://aescape-8ocoec.zitadel.cloud/oauth/v2/device_authorization\n    registration: null\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types: [code, id_token, id_token token]\n  response_modes: [query,\
  \ fragment, form_post]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post, private_key_jwt]\n  id_token_signing_algs: [EdDSA, RS256, RS384, RS512, ES256, ES384, ES512]\n  subject_types: [public]\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\n  request_parameter_supported: true\n  request_uri_parameter_supported: false\n  claims_supported: [sub, aud, exp, iat, iss, auth_time, nonce, acr, amr, c_hash, at_hash,\n    act, scopes, client_id, azp, preferred_username, name, family_name, given_name,\n    locale, email, email_verified, phone_number, phone_number_verified]\n  scopes: scopes/aescape-scopes.yml\nobservations:\n- The consumer application at app.aescape.com declares three Zitadel tenants in its\n  Content-Security-Policy — production (aescape-8ocoec), QA (aescape-qa-aotwzf) and\n  dev (aescape-dev-bi5ra8) — plus an Auth0 connect-src (*.us.auth0.com). Only the\n  production tenant is profiled\
  \ here.\n- Non-production tenants also serve a 200 OIDC discovery document but are deliberately\n  not harvested as Aescape's published contract.\n- implicit is advertised as a supported grant type by the tenant. This is the Zitadel\n  platform default and is not evidence that Aescape uses it.\ngaps:\n- No public API authentication documentation exists for api.aescape.com.\n- No API key, bearer-token or mTLS scheme is publicly documented.\n- The developer documentation that would carry an auth guide is behind HTTP Basic auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aescape/refs/heads/main/authentication/aescape-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Robotics
- Health and Wellness
- Fitness
- Massage
- Artificial Intelligence
- Consumer Hardware
- Hospitality
- Recovery
- Identity
---
