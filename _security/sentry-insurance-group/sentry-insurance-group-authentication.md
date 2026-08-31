---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sentry Insurance Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentry Insurance declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sentry Insurance
provider_slug: sentry-insurance-group
scheme_count: 2
schemes:
- dpop:
    algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    supported: true
  endpoints:
    authorization: https://account.sentry.com/oauth2/default/v1/authorize
    device_authorization: https://account.sentry.com/oauth2/default/v1/device/authorize
    dynamic_client_registration: https://account.sentry.com/oauth2/v1/clients
    end_session: https://account.sentry.com/oauth2/default/v1/logout
    introspection: https://account.sentry.com/oauth2/default/v1/introspect
    jwks: https://account.sentry.com/oauth2/default/v1/keys
    revocation: https://account.sentry.com/oauth2/default/v1/revoke
    token: https://account.sentry.com/oauth2/default/v1/token
    userinfo: https://account.sentry.com/oauth2/default/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id: sentry_okta_oidc
  id_token_signing_algs:
  - RS256
  issuer: https://account.sentry.com/oauth2/default
  observed_client:
    note: the live insight.sentry.com sign-in redirect uses response_type=code with code_challenge_method=S256 and scope "offline_access openid profile email", confirming authorization code + PKCE is the deployed flow.
    observed_at: '2026-08-29'
  openid_connect_url: https://account.sentry.com/oauth2/default/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    supported: true
  protocol: OpenID Connect 1.0
  response_types:
  - code
  - token
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- id: sentry_okta_org_oidc
  issuer: https://account.sentry.com
  note: org-level Okta authorization server; adds the `groups` scope, omits the myAccount scope family
  openid_connect_url: https://account.sentry.com/.well-known/openid-configuration
  protocol: OpenID Connect 1.0
  type: openIdConnect
slug: sentry-insurance-group-authentication
source_filename: sentry-insurance-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://account.sentry.com/oauth2/default/.well-known/openid-configuration\ndocs: https://www.sentry.com/what-we-offer/tools-and-services/online-tools-and-portals\nsummary: >-\n  Sentry Insurance publishes no product API and therefore no developer authentication\n  contract. What it does serve, anonymously and machine-readably, is the OpenID Connect\n  discovery metadata for the Okta tenant on its own domain (account.sentry.com) that\n  authenticates customers and appointed agents into insight.sentry.com. This profile\n  describes THAT authorization server verbatim from its published metadata. It is a\n  first-party portal identity provider, not an integration surface: no public client\n  registration, no documented API scopes, no developer key issuance.\napplies_to: Sentry Insurance customer / agent portal sign-in (insight.sentry.com)\nnot_a_developer_api: true\nschemes:\n  - id: sentry_okta_oidc\n    type: openIdConnect\n \
  \   protocol: OpenID Connect 1.0\n    openid_connect_url: https://account.sentry.com/oauth2/default/.well-known/openid-configuration\n    issuer: https://account.sentry.com/oauth2/default\n    endpoints:\n      authorization: https://account.sentry.com/oauth2/default/v1/authorize\n      token: https://account.sentry.com/oauth2/default/v1/token\n      userinfo: https://account.sentry.com/oauth2/default/v1/userinfo\n      jwks: https://account.sentry.com/oauth2/default/v1/keys\n      introspection: https://account.sentry.com/oauth2/default/v1/introspect\n      revocation: https://account.sentry.com/oauth2/default/v1/revoke\n      end_session: https://account.sentry.com/oauth2/default/v1/logout\n      device_authorization: https://account.sentry.com/oauth2/default/v1/device/authorize\n      dynamic_client_registration: https://account.sentry.com/oauth2/v1/clients\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n\
  \      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n    response_types: [code, token, id_token, code id_token, code token, id_token token, code id_token token]\n    pkce:\n      supported: true\n      methods: [S256]\n    dpop:\n      supported: true\n      algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    id_token_signing_algs: [RS256]\n    subject_types: [public]\n    observed_client:\n      note: >-\n        the live insight.sentry.com sign-in redirect uses response_type=code with\n        code_challenge_method=S256 and scope \"offline_access openid profile email\",\n        confirming authorization code + PKCE is the deployed flow.\n      observed_at: '2026-08-29'\n  - id: sentry_okta_org_oidc\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    openid_connect_url: https://account.sentry.com/.well-known/openid-configuration\n\
  \    issuer: https://account.sentry.com\n    note: org-level Okta authorization server; adds the `groups` scope, omits the myAccount scope family\napi_key_auth: false\nmutual_tls: false\npublic_client_registration:\n  endpoint_advertised: https://account.sentry.com/oauth2/v1/clients\n  usable_by_third_parties: unknown\n  note: >-\n    Okta advertises the RFC 7591 dynamic client registration endpoint in its metadata by\n    default; Sentry Insurance publishes no documentation offering it to third parties, so\n    no claim is made that an outside developer can register a client.\ngaps:\n  - no developer-facing authentication documentation is published anywhere on sentry.com\n  - no API key, token, or credential issuance flow is documented for partners or agents\n  - scopes are the stock Okta/OIDC set; no business-domain scopes are published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-insurance-group/refs/heads/main/authentication/sentry-insurance-group-authentication.yml
summary_line: 2 schemes
tags:
- Fortune 1000
- Insurance
- Property and Casualty Insurance
- Commercial Insurance
- Workers Compensation
- Auto Insurance
- Retirement
- Annuities
- Mutual Insurance
- Financial Services
- Trucking
- Wisconsin
- United States
---
