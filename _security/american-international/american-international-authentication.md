---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: American International Authentication
name_suffix: Authentication
oauth_flows: []
overview: American International Group (AIG) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: American International Group (AIG)
provider_slug: american-international
scheme_count: 2
schemes:
- client_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  discovery: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server
  dpop:
    algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    supported: true
  dynamic_client_registration:
    anonymous: false
    endpoint: https://auth1.customerpltfm.aig.com/oauth2/v1/clients
    note: The Okta tenant advertises an RFC 7591 registration_endpoint, but it is the standard Okta org endpoint and requires an Okta API token. It is not an open registration surface for third-party developers.
  endpoints:
    authorization: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/authorize
    device_authorization: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/device/authorize
    introspection: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/introspect
    jwks: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/keys
    logout: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/logout
    revocation: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/revoke
    token: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/token
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  header: Authorization
  id: aig_okta_oauth2
  in: header
  issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7
  pkce:
    methods:
    - S256
    supported: true
  scheme: Bearer
  standard: OAuth 2.0 (RFC 6749) + RFC 8414 authorization-server metadata
  type: oauth2
- discovery: https://auth1.customerpltfm.aig.com/.well-known/openid-configuration
  id: aig_oidc
  id_token_encryption_algs:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_signing_algs:
  - RS256
  issuer: https://auth1.customerpltfm.aig.com
  note: The org-level issuer carries the standard OIDC scope set (openid, profile, email, address, phone, offline_access, groups) plus Okta management scopes; it authenticates people into AIG's portals rather than authorizing API calls.
  standard: OpenID Connect Discovery 1.0
  type: openIdConnect
  userinfo: https://auth1.customerpltfm.aig.com/oauth2/v1/userinfo
slug: american-international-authentication
source_filename: american-international-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://auth1.customerpltfm.aig.com/.well-known/openid-configuration and\n  https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server\n  (both HTTP 200, fetched anonymously 2026-09-02), plus an anonymous probe of\n  https://commercial.api.aig.com (HTTP 403)\nprovider: American International Group (AIG)\nproviderId: american-international\nsummary: >-\n  AIG publishes no public API reference and no OpenAPI, so this profile is built entirely from the\n  identity metadata AIG's own Okta tenant serves anonymously. AIG's commercial API gateway\n  (commercial.api.aig.com) is live and rejects every unauthenticated request with a plain-text\n  403 \"You are not authorized, Forbidden, Contact AIG HD\" from an Okta-backed policy proxy.\n  Tokens are issued by AIG's customer identity platform at auth1.customerpltfm.aig.com. There is\n  no self-service signup — credentials are provisioned\
  \ to appointed brokers, producers and clients\n  through AIG's portals and distribution agreements.\nschemes:\n  - id: aig_okta_oauth2\n    type: oauth2\n    standard: OAuth 2.0 (RFC 6749) + RFC 8414 authorization-server metadata\n    in: header\n    header: Authorization\n    scheme: Bearer\n    issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7\n    discovery: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server\n    endpoints:\n      authorization: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/authorize\n      token: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/token\n      introspection: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/introspect\n      revocation: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/revoke\n      logout: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/logout\n      device_authorization:\
  \ https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/device/authorize\n      jwks: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/keys\n    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n    pkce:\n      supported: true\n      methods:\n        - S256\n    client_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    dpop:\n      supported: true\n      algs:\n        - RS256\n        - RS384\n        - RS512\n        - ES256\n        - ES384\n        - ES512\n    dynamic_client_registration:\n      endpoint: https://auth1.customerpltfm.aig.com/oauth2/v1/clients\n      anonymous: false\n      note: >-\n        The Okta tenant advertises an RFC 7591 registration_endpoint, but it is the standard\
  \ Okta\n        org endpoint and requires an Okta API token. It is not an open registration surface for\n        third-party developers.\n  - id: aig_oidc\n    type: openIdConnect\n    standard: OpenID Connect Discovery 1.0\n    issuer: https://auth1.customerpltfm.aig.com\n    discovery: https://auth1.customerpltfm.aig.com/.well-known/openid-configuration\n    id_token_signing_algs:\n      - RS256\n    id_token_encryption_algs:\n      - RSA-OAEP-256\n      - RSA-OAEP-384\n      - RSA-OAEP-512\n    userinfo: https://auth1.customerpltfm.aig.com/oauth2/v1/userinfo\n    note: >-\n      The org-level issuer carries the standard OIDC scope set (openid, profile, email, address,\n      phone, offline_access, groups) plus Okta management scopes; it authenticates people into\n      AIG's portals rather than authorizing API calls.\ngateway:\n  host: https://commercial.api.aig.com\n  anonymous_status: 403\n  anonymous_body: 'You are not authorized, Forbidden, Contact AIG HD'\n  challenge_headers:\
  \ none\n  finding: >-\n    The gateway does NOT emit an RFC 6750 WWW-Authenticate challenge or an RFC 9728\n    protected-resource-metadata pointer on its 403, so an agent that reaches the host has no\n    machine-readable way to learn where to get a token. The link between the gateway and the Okta\n    issuer had to be established by hand.\nonboarding:\n  self_service: false\n  public_signup: false\n  channel: >-\n    Credentials are provisioned through AIG's broker and producer portals (myAIG, the Producer\n    Management Portal) under a distribution or client agreement. There is no public developer\n    signup, no API key page, and no sandbox.\ngaps:\n  - No OpenAPI or public API reference documents which scheme applies to which operation.\n  - No RFC 9728 /.well-known/oauth-protected-resource on the gateway host (403 on every path).\n  - No security.txt — /.well-known/security.txt is 403 on www.aig.com and on the gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-international/refs/heads/main/authentication/american-international-authentication.yml
summary_line: 2 schemes
tags:
- Insurance
- Property Casualty
- Cyber Insurance
- Commercial Insurance
- Global Insurance
- Financial-Services
- Reinsurance
- Fortune 500
---
