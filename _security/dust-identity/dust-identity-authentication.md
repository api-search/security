---
api_key_in:
- header
api_specs:
- filename: dust-identity-apid-openapi.yml
  format: yaml
  label: DUST API
  slug: dust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/openapi/dust-identity-apid-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dust Identity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: Dust Identity secures its APIs with http, oauth2, openIdConnect, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: Dust Identity
provider_slug: dust-identity
scheme_count: 4
schemes:
- applies_to: all 177 operations of /api/v1/* (and /api/auth/*)
  bearerFormat: JWT
  description: JWT issued by the DUST auth service. Obtain one by exchanging a Service Account API key (GET /api/auth/token with the key header) or via the OAuth2 client_credentials grant. Tokens are short-lived; re-exchange on expiry.
  name: Bearer
  role: calling the DUST API
  scheme: bearer
  sources:
  - openapi/dust-identity-apid-openapi.yml
  type: http
- exchange_host: https://apid.dustid.io
  exchange_operation: GET /api/auth/token
  in: header
  name: ServiceAccountApiKey
  note: API keys are never sent to core endpoints directly — only to the token-exchange endpoint. APID proxies this to AuthD so one base URL covers both.
  parameter_name: x-api-key
  returns:
    expiresAt: null
    expiresIn: null
    token: null
  role: exchanging for a bearer token
  sources:
  - https://docs.dustid.io/api/authentication/
  type: apiKey
- client_auth:
  - client_secret_post
  - client_secret_basic
  flow: clientCredentials
  name: ServiceAccountOAuth2
  note: The resulting token is identical in shape and rights to one from the API-key exchange.
  returns: standard OAuth2 token response {access_token, token_type, expires_in}
  role: enterprise middleware integration (SAP Integration Suite, MuleSoft, Boomi)
  sources:
  - https://docs.dustid.io/api/authentication/
  tokenUrl: https://authd.dustid.io/api/auth/dust/service-accounts/token
  type: oauth2
- flows:
  - authorizationCode
  - refreshToken
  id_token_signing_alg:
  - EdDSA
  name: AuthDOpenIDConnect
  openIdConnectUrl: https://authd.dustid.io/.well-known/openid-configuration
  pkce:
  - S256
  role: interactive user sign-in to DICE and OIDC relying parties
  sources:
  - well-known/dust-identity-openid-configuration.json
  type: openIdConnect
slug: dust-identity-authentication
source_filename: dust-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.dustid.io/api/authentication/\nderived_from: openapi/dust-identity-apid-openapi.yml\ndocs: https://docs.dustid.io/api/authentication/\nnote: >-\n  The OpenAPI declares one security scheme — http/bearer/JWT applied globally to all\n  177 operations — which understates the real model. The documentation and the AuthD\n  OIDC discovery document add the credential-issuance side: a Service Account machine\n  identity holding an API key and/or an OAuth2 client, exchanged for a short-lived JWT.\n  Upgraded from the mechanical derivation with the documented model.\nsummary:\n  types: [http, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  api_key_names: [x-api-key]\n  oauth2_flows: [clientCredentials, authorizationCode, refreshToken]\n  bearer_format: JWT\n  applied: globally — every operation in the spec inherits the root security requirement\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  role: calling the DUST API\n  applies_to: all 177 operations of /api/v1/* (and /api/auth/*)\n  description: >-\n    JWT issued by the DUST auth service. Obtain one by exchanging a Service Account API\n    key (GET /api/auth/token with the key header) or via the OAuth2 client_credentials\n    grant. Tokens are short-lived; re-exchange on expiry.\n  sources: [openapi/dust-identity-apid-openapi.yml]\n- name: ServiceAccountApiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  role: exchanging for a bearer token\n  exchange_operation: GET /api/auth/token\n  exchange_host: https://apid.dustid.io\n  returns: {token, expiresIn, expiresAt}\n  sources: [https://docs.dustid.io/api/authentication/]\n  note: >-\n    API keys are never sent to core endpoints directly — only to the token-exchange\n    endpoint. APID proxies this to AuthD so one base URL covers both.\n- name: ServiceAccountOAuth2\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://authd.dustid.io/api/auth/dust/service-accounts/token\n\
  \  client_auth: [client_secret_post, client_secret_basic]\n  role: enterprise middleware integration (SAP Integration Suite, MuleSoft, Boomi)\n  returns: standard OAuth2 token response {access_token, token_type, expires_in}\n  sources: [https://docs.dustid.io/api/authentication/]\n  note: The resulting token is identical in shape and rights to one from the API-key\n    exchange.\n- name: AuthDOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://authd.dustid.io/.well-known/openid-configuration\n  role: interactive user sign-in to DICE and OIDC relying parties\n  flows: [authorizationCode, refreshToken]\n  pkce: [S256]\n  id_token_signing_alg: [EdDSA]\n  sources: [well-known/dust-identity-openid-configuration.json]\nidentity_model:\n  principal: Service Account\n  description: >-\n    A first-class machine identity that belongs to exactly one organization, can be\n    granted team access like a member, and is recorded as itself in the audit ledger\n    rather than as whichever\
  \ employee configured it. Credentials can be rotated or\n    revoked without touching any personal account. One Service Account can hold both an\n    API key and an OAuth2 client.\n  personal_api_keys: false\n  personal_api_keys_note: >-\n    Personal API keys do not exist and legacy user-owned keys no longer authenticate.\n    This is a notably strong posture — most providers still allow user-bound keys.\n  provisioning: organization admins, in the AuthD portal at https://authd.dustid.io\n    (Service accounts tab)\n  key_display: shown once at creation; DUST instructs storing it in a secrets manager\n  gating: >-\n    Service accounts must be enabled for the organization; when they are not, the tab\n    reports so and the admin is directed to support@dustidentity.com.\ntoken:\n  format: JWT\n  lifetime_seconds: 900\n  lifetime_note: documented as currently 15 minutes; DUST explicitly tells clients to\n    read expiresIn/expiresAt and not hardcode a lifetime\n  transport: 'Authorization:\
  \ Bearer <token>'\n  verification_key_source: https://apid.dustid.io/api/auth/jwks\n  verification_alternative: https://authd.dustid.io/api/auth/jwks\n  refresh: re-run the exchange; no refresh-token flow for Service Accounts\n  test_call: GET /api/v1/me\nfailure:\n  status: 401\n  body: '{\"code\":\"UNAUTHORIZED\",\"message\":\"...\",\"status\":401}'\n  see: errors/dust-identity-problem-types.yml\nauthorization:\n  model: team-membership, not scopes\n  headers: [Dust-Ctx-Org-Id, Dust-Ctx-Team-Id]\n  see: [scopes/dust-identity-scopes.yml, conventions/dust-identity-conventions.yml]\ncredential_handling:\n  server_side_only: true\n  guidance: >-\n    DUST is explicit that credentials stay server-side — the browser-side scanning\n    bridge deliberately returns raw captures and requires server-held credentials to\n    identify, verify or bind them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/authentication/dust-identity-authentication.yml
summary_line: http/oauth2/openIdConnect/apiKey · 4 schemes
tags:
- Authentication
- Identity
- Supply Chain
- Traceability
- Provenance
- Anti-Counterfeiting
- Asset Tracking
- Aerospace and Defense
- Manufacturing
- Security
---
