---
api_key_in: []
api_specs:
- filename: amber-electric-sites-api-openapi.yml
  format: yaml
  label: Amber Electric Sites API
  slug: amber-electric-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-sites-api-openapi.yml
- filename: amber-electric-state-api-openapi.yml
  format: yaml
  label: Amber Electric State API
  slug: amber-electric-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-state-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Amber Electric Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Amber Electric secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Amber Electric
provider_slug: amber-electric
scheme_count: 2
schemes:
- applies_to:
  - getSites
  - getPrices
  - getCurrentPrices
  - getUsage
  exempt:
  - operationId: getCurrentRenewables
    reason: 'The operation declares an explicit `security: []` override. Confirmed returning 200 anonymously for nsw, vic, qld and sa on 2026-07-27.'
  failure:
    body: '{"message":"Unauthorized"}'
    status: 401
  header: 'Authorization: Bearer <token>'
  issued_by: Developers tab inside the logged-in customer app at https://app.amber.com.au/developers — enable Developers Mode and click "Generate a new token". Requires an active Amber electricity account at a serviced Australian address. No developer signup, sandbox, trial key or application form exists.
  name: apiKey
  scheme: bearer
  scoped: false
  sources:
  - openapi/amber-electric-public-api-openapi.json
  surface: public-api
  type: http
- acr_values:
  - urn:cds.au:cdr:2
  claims:
  - name
  - given_name
  - family_name
  - sharing_duration
  - iss
  - sub
  - aud
  - acr
  - exp
  - iat
  - nonce
  - auth_time
  - updated_at
  client_auth_signing_algs:
  - ES256
  - PS256
  client_authentication:
  - private_key_jwt
  endpoints:
    authorization: https://public.cdr.amber.com.au/connect/authorize
    cdr_arrangement_revocation: https://secure.cdr.amber.com.au/arrangements/revoke
    introspection: https://secure.cdr.amber.com.au/connect/introspect
    jwks: https://public.cdr.amber.com.au/jwks
    pushed_authorization_request: https://secure.cdr.amber.com.au/connect/par
    registration: https://secure.cdr.amber.com.au/connect/register
    revocation: https://secure.cdr.amber.com.au/arrangements/revoke
    token: https://secure.cdr.amber.com.au/connect/token
    userinfo: https://secure.cdr.amber.com.au/userinfo
  gate: ACCC accreditation as a CDR data recipient plus a software statement assertion from the CDR Register. Unavailable to an unaccredited developer at any price.
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  id_token_signing_algs:
  - ES256
  issuer: https://public.cdr.amber.com.au
  mtls_bound_tokens: true
  name: CDR OpenID Connect
  openIdConnectUrl: https://public.cdr.amber.com.au/.well-known/openid-configuration
  par_required: true
  pkce:
  - S256
  request_object_signing_algs:
  - PS256
  response_modes:
  - jwt
  response_types:
  - code
  scope_count: 16
  scopes_detail: scopes/amber-electric-scopes.yml
  sources:
  - authentication/amber-electric-cdr-openid-configuration.json
  subject_types:
  - pairwise
  surface: cdr
  type: openIdConnect
slug: amber-electric-authentication
source_filename: amber-electric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  openapi/amber-electric-public-api-openapi.json and\n  authentication/amber-electric-cdr-openid-configuration.json (fetched\n  anonymously from https://public.cdr.amber.com.au/.well-known/openid-configuration\n  on 2026-07-27).\ndocs: https://app.amber.com.au/developers\nsummary:\n  types:\n  - http\n  - openIdConnect\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  api_key_in: []\n  anonymous_operations: 1\n  access_gate: customer-account-required (own API) / accredited-only (CDR surface)\nnote: >-\n  Two independent authentication models coexist at Amber and neither is\n  self-serve. The product API uses a single unscoped HTTP bearer token that only\n  an existing Amber electricity customer can mint from the logged-in app, with\n  one operation explicitly exempted from auth entirely. The regulated Consumer\n  Data Right surface uses the full Australian CDS security profile\
  \ — OpenID\n  Connect with mandatory pushed authorization requests, private_key_jwt client\n  authentication, PKCE S256, pairwise subjects and mTLS-bound access tokens —\n  reachable only by an ACCC-accredited data recipient.\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  surface: public-api\n  sources:\n  - openapi/amber-electric-public-api-openapi.json\n  header: 'Authorization: Bearer <token>'\n  scoped: false\n  issued_by: >-\n    Developers tab inside the logged-in customer app at\n    https://app.amber.com.au/developers — enable Developers Mode and click\n    \"Generate a new token\". Requires an active Amber electricity account at a\n    serviced Australian address. No developer signup, sandbox, trial key or\n    application form exists.\n  applies_to:\n  - getSites\n  - getPrices\n  - getCurrentPrices\n  - getUsage\n  exempt:\n  - operationId: getCurrentRenewables\n    reason: >-\n      The operation declares an explicit `security: []` override. Confirmed\n      returning\
  \ 200 anonymously for nsw, vic, qld and sa on 2026-07-27.\n  failure:\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n- name: CDR OpenID Connect\n  type: openIdConnect\n  surface: cdr\n  sources:\n  - authentication/amber-electric-cdr-openid-configuration.json\n  openIdConnectUrl: https://public.cdr.amber.com.au/.well-known/openid-configuration\n  issuer: https://public.cdr.amber.com.au\n  endpoints:\n    authorization: https://public.cdr.amber.com.au/connect/authorize\n    token: https://secure.cdr.amber.com.au/connect/token\n    pushed_authorization_request: https://secure.cdr.amber.com.au/connect/par\n    introspection: https://secure.cdr.amber.com.au/connect/introspect\n    revocation: https://secure.cdr.amber.com.au/arrangements/revoke\n    cdr_arrangement_revocation: https://secure.cdr.amber.com.au/arrangements/revoke\n    userinfo: https://secure.cdr.amber.com.au/userinfo\n    registration: https://secure.cdr.amber.com.au/connect/register\n    jwks: https://public.cdr.amber.com.au/jwks\n\
  \  grant_types: [authorization_code, client_credentials, refresh_token]\n  response_types: [code]\n  response_modes: [jwt]\n  client_authentication: [private_key_jwt]\n  client_auth_signing_algs: [ES256, PS256]\n  id_token_signing_algs: [ES256]\n  request_object_signing_algs: [PS256]\n  pkce: [S256]\n  par_required: true\n  subject_types: [pairwise]\n  mtls_bound_tokens: true\n  acr_values: ['urn:cds.au:cdr:2']\n  claims: [name, given_name, family_name, sharing_duration, iss, sub, aud, acr, exp, iat, nonce, auth_time, updated_at]\n  scope_count: 16\n  scopes_detail: scopes/amber-electric-scopes.yml\n  gate: >-\n    ACCC accreditation as a CDR data recipient plus a software statement\n    assertion from the CDR Register. Unavailable to an unaccredited developer at\n    any price.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/authentication/amber-electric-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Energy
- Australia
- Electricity
- Utilities
- Consumer Data Right
- Energy Markets
- Renewables
- Solar
- Batteries
- DER
- Smart Metering
- Wholesale Pricing
---
