---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Northern Trust Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Northern Trust secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Northern Trust
provider_slug: northern-trust
scheme_count: 2
schemes:
- authorization_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize
  id_token_signing_alg:
  - RS256
  identity_provider: Okta
  issuer: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8
  jwks_uri: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/keys
  name: NorthernTrustOIDC
  openIdConnectUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/.well-known/openid-configuration
  registration_endpoint: https://login.ntrs.com/oauth2/v1/clients
  token_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/userinfo
- flows:
  - authorizationUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  name: NorthernTrustOAuth2
  type: oauth2
slug: northern-trust-authentication
source_filename: northern-trust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/.well-known/openid-configuration\n  (live Okta OIDC discovery) + developer.ntrs.com portal review\ndocs: https://developer.ntrs.com/get-started\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: required\n  pkce_methods: [S256]\n  identity_provider: Okta\n  issuer: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8\n  api_transport: Bearer access token to the enterprise gateway (https://apiservices.ntrs.com/ent/v1)\n  gateway_api_key: >-\n    The portal additionally carries a gateway API-key header; direct\n    unauthenticated or portal-key-only calls to the gateway are rejected (401/500).\nschemes:\n- name: NorthernTrustOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/.well-known/openid-configuration\n  identity_provider: Okta\n  issuer: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8\n\
  \  authorization_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize\n  token_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token\n  userinfo_endpoint: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/userinfo\n  jwks_uri: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/keys\n  registration_endpoint: https://login.ntrs.com/oauth2/v1/clients\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n- name: NorthernTrustOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize\n    tokenUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token\n    pkce: S256\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\nnotes: >-\n  Authorization Code + PKCE (S256)\
  \ against an Okta-hosted custom authorization\n  server. private_key_jwt client authentication is supported, which is the\n  FAPI-grade confidential-client method appropriate for the institutional B2B\n  audience. Business scopes (aor.role, api.read, interclient_access) are captured\n  in scopes/northern-trust-scopes.yml. Live API access requires partner\n  registration; only the anonymous discovery metadata is public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-trust/refs/heads/main/authentication/northern-trust-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Fortune 500
- Banking
- Wealth Management
- Asset Servicing
- Asset Management
- Financial Services
- United States
---
