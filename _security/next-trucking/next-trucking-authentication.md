---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Next Trucking Authentication
name_suffix: Authentication
oauth_flows: []
overview: NEXT Trucking declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: NEXT Trucking
provider_slug: next-trucking
scheme_count: 3
schemes:
- endpoints:
    authorization: https://prod-nexttrucking.us.auth0.com/authorize
    device_authorization: https://prod-nexttrucking.us.auth0.com/oauth/device/code
    jwks: https://prod-nexttrucking.us.auth0.com/.well-known/jwks.json
    mfa_challenge: https://prod-nexttrucking.us.auth0.com/mfa/challenge
    registration: https://prod-nexttrucking.us.auth0.com/oidc/register
    revocation: https://prod-nexttrucking.us.auth0.com/oauth/revoke
    token: https://prod-nexttrucking.us.auth0.com/oauth/token
    userinfo: https://prod-nexttrucking.us.auth0.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: auth0_oidc
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://prod-nexttrucking.us.auth0.com/
  machine_to_machine:
    evidence: client_credentials is advertised in grant_types_supported, which is the grant a server-to-server integration would use — but no client registration path, audience or scope set is published for third parties, so this cannot be exercised without NEXT Trucking issuing credentials.
    supported: true
  name: NEXT Trucking Auth0 tenant (OpenID Connect)
  note: This is the tenant the ATLAS operations console and the shipper/carrier web apps authenticate against. It is a real, anonymously readable OIDC deployment, not a documented public API auth model. The scopes it advertises are the stock OIDC profile scopes (see scopes/), not NEXT-Trucking-specific API permissions.
  openIdConnectUrl: https://prod-nexttrucking.us.auth0.com/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    - plain
    supported: true
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- confidence: medium
  documented: false
  evidence: Every service path on the gateway (/shippers, /carrier, /trips, /delivery-order, /pricing-v2, /yards and 20 more discovered in the ATLAS bundle) returns nginx "401 Authorization Required" to an anonymous GET. Bearer is inferred from the Auth0 OIDC tenant the front ends obtain tokens from; the exact header form is NOT published and was not observed, so treat it as unconfirmed.
  header: Authorization
  id: gateway_bearer
  in: header
  name: ATLAS service gateway (bearer token, undocumented)
  observed_on: https://svcs.us-west-2.prod.aws.nexttrucking.com
  scheme: bearer
  type: http
- discovery: null
  documented: false
  evidence: Referenced in the ATLAS bundle. Org-level /.well-known/openid-configuration returns 404 (Okta exposes discovery per authorization server, and no server id is public). Appears to be employee SSO rather than a customer or developer identity surface.
  host: https://nexttrucking.okta.com
  id: okta_sso
  name: Okta org (workforce SSO)
  type: openIdConnect
slug: next-trucking-authentication
source_filename: next-trucking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://prod-nexttrucking.us.auth0.com/.well-known/openid-configuration (HTTP 200, saved to\n  well-known/next-trucking-openid-configuration.json); the ATLAS application bundle at\n  https://atlas.nexttrucking.com/index.05305cf32fe3cdc18fa6.js (tenant + gateway hosts); live\n  probes of https://svcs.us-west-2.prod.aws.nexttrucking.com.\nsummary: >-\n  NEXT Trucking publishes no developer authentication documentation. What is verifiable without\n  credentials is the identity layer its own applications use: an Auth0 tenant implementing OpenID\n  Connect / OAuth 2.0, and an API gateway that rejects every anonymous request with HTTP 401.\n  Everything below was read from machine-readable discovery documents or observed on the wire —\n  none of it is a published developer contract, and no key-issuance process is documented publicly.\ndocs: null\ndocs_note: >-\n  No public authentication reference exists. There is no developer\
  \ portal, no API reference and no\n  \"get an API key\" page anywhere on nexttrucking.com; the sitemap contains 23 pages and none of\n  them is developer-facing.\nschemes:\n  - id: auth0_oidc\n    type: openIdConnect\n    name: NEXT Trucking Auth0 tenant (OpenID Connect)\n    openIdConnectUrl: https://prod-nexttrucking.us.auth0.com/.well-known/openid-configuration\n    issuer: https://prod-nexttrucking.us.auth0.com/\n    endpoints:\n      authorization: https://prod-nexttrucking.us.auth0.com/authorize\n      token: https://prod-nexttrucking.us.auth0.com/oauth/token\n      userinfo: https://prod-nexttrucking.us.auth0.com/userinfo\n      jwks: https://prod-nexttrucking.us.auth0.com/.well-known/jwks.json\n      device_authorization: https://prod-nexttrucking.us.auth0.com/oauth/device/code\n      revocation: https://prod-nexttrucking.us.auth0.com/oauth/revoke\n      registration: https://prod-nexttrucking.us.auth0.com/oidc/register\n      mfa_challenge: https://prod-nexttrucking.us.auth0.com/mfa/challenge\n\
  \    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    response_types:\n      - code\n      - token\n      - id_token\n      - code token\n      - code id_token\n      - token id_token\n      - code token id_token\n    pkce:\n      supported: true\n      methods:\n        - S256\n        - plain\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - none\n    id_token_signing_algs:\n      - HS256\n      - RS256\n      - PS256\n    machine_to_machine:\n      supported: true\n      evidence: >-\n        client_credentials is advertised in grant_types_supported, which is the grant a server-to-server\n        integration would use — but no client registration path, audience or scope\
  \ set is published for\n        third parties, so this cannot be exercised without NEXT Trucking issuing credentials.\n    note: >-\n      This is the tenant the ATLAS operations console and the shipper/carrier web apps authenticate\n      against. It is a real, anonymously readable OIDC deployment, not a documented public API auth\n      model. The scopes it advertises are the stock OIDC profile scopes (see scopes/), not\n      NEXT-Trucking-specific API permissions.\n  - id: gateway_bearer\n    type: http\n    scheme: bearer\n    name: ATLAS service gateway (bearer token, undocumented)\n    in: header\n    header: Authorization\n    observed_on: https://svcs.us-west-2.prod.aws.nexttrucking.com\n    evidence: >-\n      Every service path on the gateway (/shippers, /carrier, /trips, /delivery-order, /pricing-v2,\n      /yards and 20 more discovered in the ATLAS bundle) returns nginx \"401 Authorization Required\"\n      to an anonymous GET. Bearer is inferred from the Auth0 OIDC tenant\
  \ the front ends obtain tokens\n      from; the exact header form is NOT published and was not observed, so treat it as unconfirmed.\n    confidence: medium\n    documented: false\n  - id: okta_sso\n    type: openIdConnect\n    name: Okta org (workforce SSO)\n    host: https://nexttrucking.okta.com\n    discovery: null\n    evidence: >-\n      Referenced in the ATLAS bundle. Org-level /.well-known/openid-configuration returns 404 (Okta\n      exposes discovery per authorization server, and no server id is public). Appears to be employee\n      SSO rather than a customer or developer identity surface.\n    documented: false\nmtls: false\napi_keys:\n  published: false\n  note: No API key issuance, prefix convention or key management surface is documented publicly.\ngaps:\n  - No public authentication documentation of any kind.\n  - No documented way for a third party to obtain credentials; access appears to follow a signed\n    shipper/carrier agreement rather than self-service registration.\n\
  \  - The gateway's token format, audience and required scopes are not published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-trucking/refs/heads/main/authentication/next-trucking-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Logistics
- Freight
- Trucking
- Drayage
- Supply Chain
- Transportation
- Marketplace
- Transportation Management
- Shipping
---
