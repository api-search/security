---
api_key_in: []
api_specs:
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Property API
  slug: pricefinder-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder AVM & Valuation API
  slug: pricefinder-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Sales, Rentals & Listings API
  slug: pricefinder-sales-rentals-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Suburb & Market Statistics API
  slug: pricefinder-suburb-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Title & Land Reference API
  slug: pricefinder-title-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Search & Suggest API
  slug: pricefinder-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Appraisals & CMA API
  slug: pricefinder-appraisals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Property Event Subscriptions API
  slug: pricefinder-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder SSO API
  slug: pricefinder-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder OAuth 2.0 Token API
  slug: pricefinder-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pricefinder Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: Pricefinder secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: Pricefinder
provider_slug: pricefinder
scheme_count: 1
schemes:
- declared_in_spec: false
  derived_from: POST /oauth2/token operation description (operationId getToken)
  flows:
  - credential_model: 'client_id is the API user''s Pricefinder username; client_secret is that user''s

      Pricefinder password. HTTP Basic auth is documented as an accepted alternative

      to passing username and password as form parameters.

      '
    flow: clientCredentials
    grant_type: client_credentials
    required_parameters:
    - client_id
    - client_secret
  - authorization_url: https://api.pricefinder.com.au/v1/auth/authorize.html
    authorization_url_status: 200
    callback_denied: '{redirect_uri}?error=access_denied'
    callback_success: '{redirect_uri}?state=<state>&code=<authorization_code>'
    flow: authorizationCode
    grant_type: authorization_code
    https_required: true
    note: 'Three-legged delegated authorization — used to act on another Pricefinder

      user''s behalf. The hosted authorize page renders a "PriceFinder Login" screen

      and is reachable anonymously (probed 200, 2026-07-26).

      '
    request_parameters:
    - client_id
    - state
    - redirect_uri
    required_parameters:
    - client_id
    - client_secret
    - redirect_uri
    - code
  - flow: refreshToken
    grant_type: refresh_token
    note: Consumes the refresh token and returns BOTH a new access token and a new refresh token (rotating refresh tokens).
    required_parameters:
    - client_id
    - client_secret
    - refresh_token
  name: pricefinder_oauth2
  scopes: []
  scopes_note: 'NO SCOPES. The contract defines no scope vocabulary, the token request accepts no

    `scope` parameter, and no scopes/permissions reference page exists on any

    Pricefinder surface. Authorization is all-or-nothing per credentialed user, with

    entitlement enforced server-side by commercial subscription (see GET /features,

    operationId getFeatures, which returns the calling user''s UserFeatures

    entitlement set). This is why no scopes/ artifact is emitted for Pricefinder.

    '
  token_endpoint: https://api.pricefinder.com.au/v1/oauth2/token
  token_endpoint_method: POST
  token_request_content_type: application/x-www-form-urlencoded
  type: oauth2
slug: pricefinder-authentication
source_filename: pricefinder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: |\n  POST /oauth2/token operation description (HTML prose) in\n  openapi/pricefinder-api-swagger.json, plus live probes of\n  https://api.pricefinder.com.au/v1/auth/authorize.html (200) and\n  https://api.pricefinder.com.au/.well-known/openid-configuration (404), 2026-07-26.\ndocs: https://api.pricefinder.com.au/v1/swagger/index.html\n\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode, refreshToken]\n  http_schemes: [basic, bearer]\n  self_serve: false\n  gate: application-approval — credentials are issued only under a negotiated\n    commercial subscription; there is no developer signup, free tier or sandbox key.\n\nspec_gap: |\n  THE CONTRACT DECLARES NO securityDefinitions AND NO security BLOCK. This profile\n  could not be derived mechanically (0-working/derive-authentication.py returned zero\n  schemes for this provider) because the Swagger 2.0 document carries no security\n\
  \  metadata at all — despite every one of its 116 operations requiring a bearer token.\n  The entire OAuth 2.0 model is described in HTML prose inside a single operation\n  description. A machine reading this contract cannot determine how to authenticate;\n  a human has to read the rendered description field. This profile is the\n  human-readable model transcribed into machine-readable form by API Evangelist, and\n  is the correct target shape for a securityDefinitions block Pricefinder should\n  publish.\n\nschemes:\n- name: pricefinder_oauth2\n  type: oauth2\n  declared_in_spec: false\n  derived_from: POST /oauth2/token operation description (operationId getToken)\n  token_endpoint: https://api.pricefinder.com.au/v1/oauth2/token\n  token_endpoint_method: POST\n  token_request_content_type: application/x-www-form-urlencoded\n  flows:\n  - flow: clientCredentials\n    grant_type: client_credentials\n    required_parameters: [client_id, client_secret]\n    credential_model: |\n      client_id\
  \ is the API user's Pricefinder username; client_secret is that user's\n      Pricefinder password. HTTP Basic auth is documented as an accepted alternative\n      to passing username and password as form parameters.\n  - flow: authorizationCode\n    grant_type: authorization_code\n    authorization_url: https://api.pricefinder.com.au/v1/auth/authorize.html\n    authorization_url_status: 200\n    required_parameters: [client_id, client_secret, redirect_uri, code]\n    request_parameters: [client_id, state, redirect_uri]\n    https_required: true\n    callback_success: \"{redirect_uri}?state=<state>&code=<authorization_code>\"\n    callback_denied: \"{redirect_uri}?error=access_denied\"\n    note: |\n      Three-legged delegated authorization — used to act on another Pricefinder\n      user's behalf. The hosted authorize page renders a \"PriceFinder Login\" screen\n      and is reachable anonymously (probed 200, 2026-07-26).\n  - flow: refreshToken\n    grant_type: refresh_token\n    required_parameters:\
  \ [client_id, client_secret, refresh_token]\n    note: Consumes the refresh token and returns BOTH a new access token and a new\n      refresh token (rotating refresh tokens).\n  scopes: []\n  scopes_note: |\n    NO SCOPES. The contract defines no scope vocabulary, the token request accepts no\n    `scope` parameter, and no scopes/permissions reference page exists on any\n    Pricefinder surface. Authorization is all-or-nothing per credentialed user, with\n    entitlement enforced server-side by commercial subscription (see GET /features,\n    operationId getFeatures, which returns the calling user's UserFeatures\n    entitlement set). This is why no scopes/ artifact is emitted for Pricefinder.\n\ntoken_presentation:\n- style: header\n  example: 'Authorization: Bearer <access_token>'\n  preferred: true\n- style: query\n  example: '?access_token=<access_token>'\n  note: |\n    Documented as a first-class alternative. Bearer tokens in query strings are\n    logged by proxies and appear in\
  \ browser history and referrer headers — RFC 6750\n    section 5.3 and RFC 6819 both discourage it. Recorded as observed, not endorsed.\n\ntoken_response:\n  schema: openapi/pricefinder-api-swagger.json#/definitions/ClientAccessToken\n  fields:\n  - {name: access_token, type: string}\n  - {name: token_type, type: string}\n  - {name: expires_in, type: string, note: typed as string, not integer, in the\n      contract}\n  - {name: refresh_token, type: string}\n\ntoken_endpoint_errors:\n- {status: 401, description: Invalid username/password}\n- {status: 400, description: Bad Request}\n\nopenid_connect:\n  supported: false\n  discovery_probe:\n    url: https://api.pricefinder.com.au/.well-known/openid-configuration\n    status: 404\n    date: '2026-07-26'\n  authorization_server_metadata_probe:\n    url: https://api.pricefinder.com.au/.well-known/oauth-authorization-server\n    status: 404\n    date: '2026-07-26'\n\nmutual_tls: false\napi_keys: false\n\nenforcement_evidence:\n- {probe: 'GET\
  \ https://api.pricefinder.com.au/v1/features', status: 401,\n   note: Anonymous call to a data path rejected.}\n- {probe: 'GET https://api.pricefinder.com.au/v1/stubs/java', status: 401,\n   note: Even the client-library generator requires a token.}\n- {probe: 'POST https://api.pricefinder.com.au/v1/oauth2/token (no credentials)',\n   status: 401, note: The token endpoint itself rejects anonymous callers.}\n- {probe: 'GET https://api.pricefinder.com.au/v1/swagger.json', status: 200,\n   note: The CONTRACT is anonymous. The gate is on data, not on discovery.}\n\nrelated:\n  conventions: conventions/pricefinder-conventions.yml\n  conformance: conformance/pricefinder-conformance.yml\n  well_known: well-known/pricefinder-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/authentication/pricefinder-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real Estate
- Australia
- PropTech
- Property Data
- Valuation
- AVM
- Property Listings
- Rentals
- Land Registry
- Title
- Mortgage
- Market Data
---
