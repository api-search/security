---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Psc Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
overview: PSC Insurance secures its APIs with openIdConnect, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, and tokenExchange flow(s).
provider_name: PSC Insurance
provider_slug: psc-insurance
scheme_count: 3
schemes:
- backchannel_logout: true
  caveat: 'Every value above is emitted by the Auth0 tenant discovery document. These are

    tenant capabilities, not a documented PSC authorization contract. No PSC

    resource server, audience or product scope is published anywhere. Do not read

    the advertised grant types as evidence of a machine-to-machine API programme.

    '
  dpop:
    signing_alg_values:
    - ES256
    supported: true
  endpoints:
    authorization: https://login.pscinsurance.com.au/authorize
    backchannel_authentication: https://login.pscinsurance.com.au/bc-authorize
    device_authorization: https://login.pscinsurance.com.au/oauth/device/code
    end_session: https://login.pscinsurance.com.au/oidc/logout
    jwks: https://login.pscinsurance.com.au/.well-known/jwks.json
    mfa_challenge: https://login.pscinsurance.com.au/mfa/challenge
    registration: https://login.pscinsurance.com.au/oidc/register
    revocation: https://login.pscinsurance.com.au/oauth/revoke
    token: https://login.pscinsurance.com.au/oauth/token
    userinfo: https://login.pscinsurance.com.au/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_alg_values:
  - HS256
  - RS256
  - PS256
  issuer: https://login.pscinsurance.com.au/
  mfa:
    evidence: mfa_challenge_endpoint advertised; MFA grant types advertised
    supported: true
  name: PSCIdentity
  openIdConnectUrl: https://login.pscinsurance.com.au/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  provider: Auth0 (custom domain, Australia region)
  sources:
  - well-known/psc-insurance-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- host: https://tw8a70my.api.sanity.io
  name: SanityContentLakeAnonymousRead
  note: 'The Sanity Content Lake project (tw8a70my) dataset "production" that backs

    www.pscinsurance.com.au answers GROQ query, single-document, dataset-export and

    real-time listen requests with no credential at all. This is the standard Sanity

    "public dataset" configuration for a headless marketing site, not a PSC access

    grant, and it is undocumented by PSC.

    '
  scheme: anonymous
  sources:
  - live probe 2026-07-25
  type: none
  verified_anonymous:
  - path: /v2021-10-21/data/query/production
    status: 200
  - path: /v2021-10-21/data/doc/production/{documentId}
    status: 200
  - path: /v2021-10-21/data/export/production
    status: 200
  - path: /v2021-10-21/data/listen/production
    status: 200
- name: SanityContentLakeBearer
  note: 'Write and administrative paths are token-gated: /v2021-10-21/data/mutate/production

    rejects an anonymous GET with 405 and the project management endpoint

    /v2021-10-21/projects/tw8a70my returns 401 "A valid session is required for this

    endpoint". No token is published and none was attempted.

    '
  scheme: bearer
  sources:
  - live probe 2026-07-25
  type: http
slug: psc-insurance-authentication
source_filename: psc-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.pscinsurance.com.au/.well-known/openid-configuration\ndocs: null\nnote: |\n  PSC Insurance publishes no API and therefore no API authentication documentation.\n  This profile is derived entirely from machine-readable metadata fetched\n  anonymously from the two machine-facing surfaces that do exist. Neither is a\n  documented PSC developer product: the first is the Auth0 identity boundary in\n  front of a gated client/broker login, the second is the public read side of the\n  Sanity Content Lake that backs the marketing website.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  - tokenExchange\n  anonymous_read_surfaces: 1\nschemes:\n- name: PSCIdentity\n  type: openIdConnect\n  openIdConnectUrl: https://login.pscinsurance.com.au/.well-known/openid-configuration\n  issuer: https://login.pscinsurance.com.au/\n\
  \  provider: Auth0 (custom domain, Australia region)\n  sources:\n  - well-known/psc-insurance-openid-configuration.json\n  endpoints:\n    authorization: https://login.pscinsurance.com.au/authorize\n    token: https://login.pscinsurance.com.au/oauth/token\n    userinfo: https://login.pscinsurance.com.au/userinfo\n    jwks: https://login.pscinsurance.com.au/.well-known/jwks.json\n    revocation: https://login.pscinsurance.com.au/oauth/revoke\n    registration: https://login.pscinsurance.com.au/oidc/register\n    device_authorization: https://login.pscinsurance.com.au/oauth/device/code\n    backchannel_authentication: https://login.pscinsurance.com.au/bc-authorize\n    end_session: https://login.pscinsurance.com.au/oidc/logout\n    mfa_challenge: https://login.pscinsurance.com.au/mfa/challenge\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values:\n  - HS256\n  - RS256\n  - PS256\n  pkce:\n    supported:\
  \ true\n    code_challenge_methods:\n    - S256\n    - plain\n  dpop:\n    supported: true\n    signing_alg_values:\n    - ES256\n  mfa:\n    supported: true\n    evidence: mfa_challenge_endpoint advertised; MFA grant types advertised\n  backchannel_logout: true\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  caveat: |\n    Every value above is emitted by the Auth0 tenant discovery document. These are\n    tenant capabilities, not a documented PSC authorization contract. No PSC\n    resource server, audience or product\
  \ scope is published anywhere. Do not read\n    the advertised grant types as evidence of a machine-to-machine API programme.\n- name: SanityContentLakeAnonymousRead\n  type: none\n  scheme: anonymous\n  sources:\n  - live probe 2026-07-25\n  host: https://tw8a70my.api.sanity.io\n  note: |\n    The Sanity Content Lake project (tw8a70my) dataset \"production\" that backs\n    www.pscinsurance.com.au answers GROQ query, single-document, dataset-export and\n    real-time listen requests with no credential at all. This is the standard Sanity\n    \"public dataset\" configuration for a headless marketing site, not a PSC access\n    grant, and it is undocumented by PSC.\n  verified_anonymous:\n  - {path: '/v2021-10-21/data/query/production', status: 200}\n  - {path: '/v2021-10-21/data/doc/production/{documentId}', status: 200}\n  - {path: '/v2021-10-21/data/export/production', status: 200}\n  - {path: '/v2021-10-21/data/listen/production', status: 200}\n- name: SanityContentLakeBearer\n  type:\
  \ http\n  scheme: bearer\n  sources:\n  - live probe 2026-07-25\n  note: |\n    Write and administrative paths are token-gated: /v2021-10-21/data/mutate/production\n    rejects an anonymous GET with 405 and the project management endpoint\n    /v2021-10-21/projects/tw8a70my returns 401 \"A valid session is required for this\n    endpoint\". No token is published and none was attempted.\nrelated:\n- scopes/psc-insurance-scopes.yml\n- well-known/psc-insurance-well-known.yml\n- conformance/psc-insurance-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/psc-insurance/refs/heads/main/authentication/psc-insurance-authentication.yml
summary_line: openIdConnect/oauth2/http · 3 schemes
tags:
- Insurance
- Australia
- Broker
- Insurance Brokerage
- Property and Casualty
- Commercial Insurance
- Cyber Insurance
- Intermediary
- Partner Gated
- No Public API
---
