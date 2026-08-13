---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Firefly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firefly secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firefly
provider_slug: firefly
scheme_count: 1
schemes:
- claims:
  - aud
  - auth_time
  - created_at
  - email
  - email_verified
  - exp
  - family_name
  - given_name
  - iat
  - identities
  - iss
  - name
  - nickname
  - phone_number
  - picture
  - sub
  description: OpenID Connect discovery for the Firefly advertiser dashboard tenant. Verified live 2026-08-12, HTTP 200, application/json, 2,501 bytes. Saved verbatim at well-known/firefly-openid-configuration.json. The RFC 8414 OAuth authorization-server metadata document at /.well-known/oauth-authorization-server is byte-identical.
  endpoints:
    authorization: https://auth.fireflyon.com/authorize
    backchannel_authentication: https://auth.fireflyon.com/bc-authorize
    device_authorization: https://auth.fireflyon.com/oauth/device/code
    dynamic_client_registration: https://auth.fireflyon.com/oidc/register
    jwks: https://auth.fireflyon.com/.well-known/jwks.json
    mfa_challenge: https://auth.fireflyon.com/mfa/challenge
    revocation: https://auth.fireflyon.com/oauth/revoke
    token: https://auth.fireflyon.com/oauth/token
    userinfo: https://auth.fireflyon.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.fireflyon.com/
  name: firefly-dashboard-oidc
  openIdConnectUrl: https://auth.fireflyon.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  scopes: scopes/firefly-scopes.yml
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
slug: firefly-authentication
source_filename: firefly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.fireflyon.com/.well-known/openid-configuration\ndocs: null\nscope_of_this_artifact: >-\n  This describes the identity layer in front of the Firefly advertiser dashboard\n  (app.fireflyon.com) and its API gateway (app-gw.api.fireflyon.com) — NOT a public\n  Firefly developer API. Firefly publishes no developer portal, no API reference and\n  no OpenAPI; see x-coverage in apis.yml. The document below was read verbatim from a\n  live, unauthenticated GET of the OpenID Connect discovery endpoint on Firefly's own\n  auth host, so every value here is Firefly-served fact rather than derivation.\n  The endpoint set is an Auth0 custom-domain tenant\n  (auth.fireflyon.com CNAME -> fireflyon-cd-p4enovzjyobijetz.edge.tenants.auth0.com),\n  which means the surface reflects Auth0 platform defaults; Firefly-specific choices\n  cannot be separated from platform defaults without authenticated access.\nsummary:\n  types:\n  - oauth2\n\
  \  - openIdConnect\n  primary: OpenID Connect (Authorization Code + PKCE) against an Auth0 custom-domain tenant\n  api_key_auth: false\n  mutual_tls: false\nschemes:\n- name: firefly-dashboard-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.fireflyon.com/.well-known/openid-configuration\n  issuer: https://auth.fireflyon.com/\n  description: >-\n    OpenID Connect discovery for the Firefly advertiser dashboard tenant. Verified live\n    2026-08-12, HTTP 200, application/json, 2,501 bytes. Saved verbatim at\n    well-known/firefly-openid-configuration.json. The RFC 8414 OAuth authorization-server\n    metadata document at /.well-known/oauth-authorization-server is byte-identical.\n  endpoints:\n    authorization: https://auth.fireflyon.com/authorize\n    token: https://auth.fireflyon.com/oauth/token\n    userinfo: https://auth.fireflyon.com/userinfo\n    jwks: https://auth.fireflyon.com/.well-known/jwks.json\n    revocation: https://auth.fireflyon.com/oauth/revoke\n    device_authorization:\
  \ https://auth.fireflyon.com/oauth/device/code\n    dynamic_client_registration: https://auth.fireflyon.com/oidc/register\n    backchannel_authentication: https://auth.fireflyon.com/bc-authorize\n    mfa_challenge: https://auth.fireflyon.com/mfa/challenge\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  response_modes:\n  - query\n  - fragment\n  - form_post\n  pkce:\n    supported: true\n\
  \    code_challenge_methods:\n    - S256\n    - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs:\n  - RS256\n  - RS384\n  - PS256\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  subject_types:\n  - public\n  claims:\n  - aud\n  - auth_time\n  - created_at\n  - email\n  - email_verified\n  - exp\n  - family_name\n  - given_name\n  - iat\n  - identities\n  - iss\n  - name\n  - nickname\n  - phone_number\n  - picture\n  - sub\n  scopes: scopes/firefly-scopes.yml\naudiences:\n- audience: https://gw.fireflyon.com\n  used_by: https://app.fireflyon.com (Firefly advertiser dashboard SPA)\n  source: >-\n    window.REACT_APP_AUTH0_AUDIENCE in the public SPA runtime config at\n    https://app.fireflyon.com/config.js (HTTP 200). The audience hostname\n    gw.fireflyon.com does not itself resolve in DNS; the gateway the SPA calls is\n    https://app-gw.api.fireflyon.com.\n  note:\
  \ >-\n    Access tokens minted for this audience are what the advertiser dashboard presents to\n    app-gw.api.fireflyon.com. That gateway answers 404 text/plain \"404 page not found\"\n    to every unauthenticated path probed, so its operation set cannot be read without\n    an advertiser account.\ngaps:\n- id: no-public-auth-documentation\n  detail: >-\n    Firefly publishes no authentication guide, no key/credential issuance page and no\n    developer portal. The only machine-readable auth surface is the Auth0 discovery\n    document above, which is platform-generated rather than Firefly-authored prose.\n  evidence:\n  - url: https://www.fireflyon.com/sitemap.xml\n    status: 200\n    note: 90 URLs, none developer- or API-facing.\n- id: no-protected-resource-metadata\n  detail: >-\n    No RFC 9728 OAuth protected-resource metadata is served by the gateway, so a client\n    cannot discover which authorization server protects app-gw.api.fireflyon.com without\n    reading the SPA config.\n\
  \  evidence:\n  - url: https://app-gw.api.fireflyon.com/.well-known/oauth-protected-resource\n    status: 404\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://auth.fireflyon.com/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.fireflyon.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://auth.fireflyon.com/.well-known/zzz-nonexistent-abc\n    status: 404\n    note: control probe — this host does not answer /.well-known/* with a catch-all.\n  - url: https://app-gw.api.fireflyon.com/.well-known/oauth-protected-resource\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firefly/refs/heads/main/authentication/firefly-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Advertising
- Digital Out-of-Home
- DOOH
- Mobility
- Advertising Technology
- AdTech
- Marketing
- Measurement
- Programmatic Advertising
---
