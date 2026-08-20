---
api_key_in: []
api_specs:
- filename: steadfast-group-flood-risk-tracker-openapi.yml
  format: yaml
  label: Steadfast Flood Risk Tracker API
  slug: flood-risk-tracker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-flood-risk-tracker-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Steadfast Group Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
- password
- device_code
- ciba
overview: Steadfast Group secures its APIs with none, openIdConnect, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refresh_token, password, device_code, and ciba flow(s).
provider_name: Steadfast Group
provider_slug: steadfast-group
scheme_count: 2
schemes:
- applies_to:
  - openapi/steadfast-group-flood-risk-tracker-openapi.yml
  description: The Flood Risk Tracker API accepts anonymous requests. No API key, bearer token, cookie or signed header was required for any observed call; sending none returned 200. Access is instead shaped by a restrictive CORS policy - the observed access-control-allow-origin is https://steadfastinsurance.wufoo.com - plus Cloudflare fronting and reCAPTCHA Enterprise on the human web form (the reCAPTCHA gate is enforced client-side in the tool's own JavaScript, not by the API).
  name: none
  sources:
  - live anonymous probes 2026-07-25
  type: none
- description: Okta-hosted OpenID Connect provider (issuer https://idp.steadfast.com.au). Serves the credentialed broker portal at broker.steadfast.com.au and, by inference from the shared estate, internal and partner applications. Discovery is public; client registration is not self-serve in practice - the dynamic client registration endpoint exists but returned 403 "Invalid session" to an anonymous request.
  dpop:
    signing_algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    supported: true
  endpoints:
    authorization: https://idp.steadfast.com.au/oauth2/v1/authorize
    device_authorization: https://idp.steadfast.com.au/oauth2/v1/device/authorize
    end_session: https://idp.steadfast.com.au/oauth2/v1/logout
    introspection: https://idp.steadfast.com.au/oauth2/v1/introspect
    issuer: https://idp.steadfast.com.au
    jwks: https://idp.steadfast.com.au/oauth2/v1/keys
    registration: https://idp.steadfast.com.au/oauth2/v1/clients
    revocation: https://idp.steadfast.com.au/oauth2/v1/revoke
    token: https://idp.steadfast.com.au/oauth2/v1/token
    userinfo: https://idp.steadfast.com.au/oauth2/v1/userinfo
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:okta:params:oauth:grant-type:otp
  - urn:okta:params:oauth:grant-type:oob
  id_token_signing_alg_values_supported:
  - RS256
  name: SteadfastIdP
  openIdConnectUrl: https://idp.steadfast.com.au/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  request_parameter_supported: true
  response_types_supported:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  scopes: scopes/steadfast-group-scopes.yml
  sources:
  - well-known/steadfast-group-openid-configuration.json
  - well-known/steadfast-group-oauth-authorization-server.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
slug: steadfast-group-authentication
source_filename: steadfast-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://idp.steadfast.com.au/.well-known/openid-configuration\ndocs: null\nsummary:\n  types:\n    - none\n    - openIdConnect\n    - oauth2\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - implicit\n    - refresh_token\n    - password\n    - device_code\n    - ciba\n  note: >-\n    Steadfast Group operates two very different authentication postures. The one genuinely\n    public API - the Flood Risk Tracker - requires and accepts NO authentication at all. Every\n    other surface (the broker portal, the partner API host, internal applications) sits behind\n    an Okta-hosted OpenID Connect provider at idp.steadfast.com.au whose discovery document is\n    anonymously readable, but whose client credentials are issued commercially rather than\n    through self-serve signup. There is no published developer authentication guide anywhere on\n    the Steadfast estate - this profile was assembled from live discovery\
  \ documents and probes,\n    not from documentation.\nschemes:\n  - name: none\n    type: none\n    description: >-\n      The Flood Risk Tracker API accepts anonymous requests. No API key, bearer token, cookie or\n      signed header was required for any observed call; sending none returned 200. Access is\n      instead shaped by a restrictive CORS policy - the observed access-control-allow-origin is\n      https://steadfastinsurance.wufoo.com - plus Cloudflare fronting and reCAPTCHA Enterprise\n      on the human web form (the reCAPTCHA gate is enforced client-side in the tool's own\n      JavaScript, not by the API).\n    applies_to:\n      - openapi/steadfast-group-flood-risk-tracker-openapi.yml\n    sources:\n      - live anonymous probes 2026-07-25\n  - name: SteadfastIdP\n    type: openIdConnect\n    openIdConnectUrl: https://idp.steadfast.com.au/.well-known/openid-configuration\n    description: >-\n      Okta-hosted OpenID Connect provider (issuer https://idp.steadfast.com.au).\
  \ Serves the\n      credentialed broker portal at broker.steadfast.com.au and, by inference from the shared\n      estate, internal and partner applications. Discovery is public; client registration is not\n      self-serve in practice - the dynamic client registration endpoint exists but returned 403\n      \"Invalid session\" to an anonymous request.\n    endpoints:\n      issuer: https://idp.steadfast.com.au\n      authorization: https://idp.steadfast.com.au/oauth2/v1/authorize\n      token: https://idp.steadfast.com.au/oauth2/v1/token\n      userinfo: https://idp.steadfast.com.au/oauth2/v1/userinfo\n      jwks: https://idp.steadfast.com.au/oauth2/v1/keys\n      introspection: https://idp.steadfast.com.au/oauth2/v1/introspect\n      revocation: https://idp.steadfast.com.au/oauth2/v1/revoke\n      end_session: https://idp.steadfast.com.au/oauth2/v1/logout\n      device_authorization: https://idp.steadfast.com.au/oauth2/v1/device/authorize\n      registration: https://idp.steadfast.com.au/oauth2/v1/clients\n\
  \    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n      - urn:okta:params:oauth:grant-type:otp\n      - urn:okta:params:oauth:grant-type:oob\n    response_types_supported:\n      - code\n      - id_token\n      - code id_token\n      - code token\n      - id_token token\n      - code id_token token\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    pkce:\n      supported: true\n      code_challenge_methods:\n        - S256\n    dpop:\n      supported: true\n      signing_algs:\n        - RS256\n        - RS384\n        - RS512\n        - ES256\n        - ES384\n        - ES512\n    id_token_signing_alg_values_supported:\n      - RS256\n    subject_types_supported:\n      - public\n    request_parameter_supported:\
  \ true\n    scopes: scopes/steadfast-group-scopes.yml\n    sources:\n      - well-known/steadfast-group-openid-configuration.json\n      - well-known/steadfast-group-oauth-authorization-server.json\nobservations:\n  - >-\n    PKCE with S256 and DPoP proof-of-possession are both advertised - a modern posture for a\n    broker-network identity provider, and stronger than the estate's published documentation\n    (of which there is none) would suggest.\n  - >-\n    The Resource Owner Password Credentials grant (`password`) and the `implicit` response types\n    remain enabled. Both are discouraged by OAuth 2.1 and BCP 212; their presence is recorded as\n    observed configuration, not as a recommendation.\n  - >-\n    `token_endpoint_auth_methods_supported` includes `none`, meaning public clients (SPA/mobile)\n    are provisioned on this tenant alongside confidential clients using private_key_jwt.\n  - >-\n    No mutualTLS, no API-key scheme and no HTTP basic scheme is published anywhere\
  \ on the\n    Steadfast estate.\ngaps:\n  - No developer-facing authentication documentation exists on any public Steadfast property.\n  - >-\n    api.steadfast.com.au - the partner API host - publishes no auth metadata; /.well-known/\n    returns 503 and the root returns 403, so its token model is not externally observable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/authentication/steadfast-group-authentication.yml
summary_line: none/openIdConnect/oauth2 · 2 schemes
tags:
- Insurance
- Australia
- Brokers
- Insurance Broker Network
- General Insurance
- Property and Casualty
- Underwriting Agency
- Agency Management
- ACORD
- Partner Gated
- New Zealand
---
