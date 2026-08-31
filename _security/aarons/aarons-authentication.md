---
api_key_in: []
api_specs:
- filename: aarons-hpp-openapi.json
  format: json
  label: Aaron's Hosted Payment Page (HPP)
  slug: aarons-hpp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-hpp-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Aarons Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aaron's declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Aaron's
provider_slug: aarons
scheme_count: 3
schemes:
- api: aarons:aarons-hpp
  applied: per-operation
  description: Declared in the HPP Swagger 2.0 document as securityDefinitions.Bearer, an apiKey scheme carried in the Authorization header. Applied at operation level on every non-ping operation.
  id: hpp-bearer
  in: header
  name: Authorization
  scheme_name: Bearer
  source: openapi/aarons-hpp-openapi.json#/securityDefinitions/Bearer
  token_issuance: Not publicly documented. The contract itself exposes /MemoryBearerToken and /CreateToken operations, implying tokens are minted by Aaron's for its own session flow rather than issued to third-party developers.
  type: apiKey
- authorization_endpoint: https://login.aarons.com/oauth2/v1/authorize
  description: Okta org authorization server on Aaron's custom domain. Anonymous OIDC discovery is served.
  discovery: well-known/aarons-login-openid-configuration.json
  end_session_endpoint: https://login.aarons.com/oauth2/v1/logout
  id: okta-oidc
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://login.aarons.com/oauth2/v1/introspect
  issuer: https://login.aarons.com
  jwks_uri: https://login.aarons.com/oauth2/v1/keys
  pkce:
  - S256
  registration_endpoint: https://login.aarons.com/oauth2/v1/clients
  revocation_endpoint: https://login.aarons.com/oauth2/v1/revoke
  token_endpoint: https://login.aarons.com/oauth2/v1/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://login.aarons.com/oauth2/v1/userinfo
- description: The custom authorization server the myaccount.aarons.com application names as its issuer. This is the one that carries Aaron's own application scope (interclient_access) alongside the standard OIDC set.
  discovery: well-known/aarons-login-default-openid-configuration.json
  id: okta-oidc-default
  issuer: https://login.aarons.com/oauth2/default
  source: https://myaccount.aarons.com/assets/index-CNr2NkAf.js — Aaron's own published application bundle names https://login.aarons.com/oauth2/default as the issuer.
  type: openIdConnect
slug: aarons-authentication
source_filename: aarons-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  openapi/aarons-hpp-openapi.json (securityDefinitions) +\n  https://login.aarons.com/.well-known/openid-configuration +\n  https://login.aarons.com/oauth2/default/.well-known/openid-configuration\nprovider: Aaron's\nproviderId: aarons\nsummary: >-\n  Aaron's runs two distinct authentication models and publishes neither as developer documentation.\n  Customer-facing identity is Okta on a custom domain (login.aarons.com) speaking OpenID Connect and\n  OAuth 2.0, with anonymous discovery documents that are fully machine-readable. The one published\n  API contract — the Hosted Payment Page service at hpp.aarons.com — declares a single bearer-token\n  scheme in its own Swagger document. There is no public developer program, no key issuance flow,\n  and no documented way for a third party to obtain either credential.\nschemes:\n  - id: hpp-bearer\n    api: aarons:aarons-hpp\n    type: apiKey\n    in: header\n    name: Authorization\n\
  \    scheme_name: Bearer\n    description: >-\n      Declared in the HPP Swagger 2.0 document as securityDefinitions.Bearer, an apiKey scheme\n      carried in the Authorization header. Applied at operation level on every non-ping operation.\n    applied: per-operation\n    source: openapi/aarons-hpp-openapi.json#/securityDefinitions/Bearer\n    token_issuance: >-\n      Not publicly documented. The contract itself exposes /MemoryBearerToken and /CreateToken\n      operations, implying tokens are minted by Aaron's for its own session flow rather than issued\n      to third-party developers.\n  - id: okta-oidc\n    type: openIdConnect\n    issuer: https://login.aarons.com\n    discovery: well-known/aarons-login-openid-configuration.json\n    description: >-\n      Okta org authorization server on Aaron's custom domain. Anonymous OIDC discovery is served.\n    authorization_endpoint: https://login.aarons.com/oauth2/v1/authorize\n    token_endpoint: https://login.aarons.com/oauth2/v1/token\n\
  \    userinfo_endpoint: https://login.aarons.com/oauth2/v1/userinfo\n    jwks_uri: https://login.aarons.com/oauth2/v1/keys\n    introspection_endpoint: https://login.aarons.com/oauth2/v1/introspect\n    revocation_endpoint: https://login.aarons.com/oauth2/v1/revoke\n    end_session_endpoint: https://login.aarons.com/oauth2/v1/logout\n    registration_endpoint: https://login.aarons.com/oauth2/v1/clients\n    id_token_signing_alg: [RS256]\n    pkce: [S256]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n  - id: okta-oidc-default\n    type: openIdConnect\n    issuer: https://login.aarons.com/oauth2/default\n    discovery: well-known/aarons-login-default-openid-configuration.json\n    description: >-\n      The custom authorization server the myaccount.aarons.com application names as its issuer.\n      This is the one that carries Aaron's own application scope (interclient_access)\
  \ alongside the\n      standard OIDC set.\n    source: >-\n      https://myaccount.aarons.com/assets/index-CNr2NkAf.js — Aaron's own published application\n      bundle names https://login.aarons.com/oauth2/default as the issuer.\ngrant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials      # org authorization server only\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\nmfa:\n  supported: true\n  evidence: >-\n    Okta MFA grant types are advertised in discovery (urn:okta:params:oauth:grant-type:otp,\n    urn:okta:params:oauth:grant-type:oob, and the auth0 mfa-otp / mfa-oob equivalents).\ngaps:\n  - No published authentication documentation for developers on any Aaron's property.\n  - No API key self-service, no developer portal, no credential request flow.\n  - HPP bearer tokens have no documented lifetime, rotation, or scope model.\ndocs: null\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/authentication/aarons-authentication.yml
summary_line: 3 schemes
tags:
- Lease-to-Own
- Retail
- Furniture
- Electronics
- Appliances
- Consumer Finance
- Fortune 1000
---
