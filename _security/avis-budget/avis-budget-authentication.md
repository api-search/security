---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avis-budget-rental-cars-openapi.yml
  format: yaml
  label: Avis Budget Group Rental Cars API
  slug: avis-budget-group-rental-cars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/openapi/avis-budget-rental-cars-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Avis Budget Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Avis Budget Group secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Avis Budget Group
provider_slug: avis-budget
scheme_count: 1
schemes:
- api_request_headers:
  - name: Authorization
    value: Bearer <access_token>
  - name: client_id
    note: Declared as a required header parameter on all 9 operations in the OpenAPI.
    value: <client_id>
  description: OAuth 2.0 client credentials flow used to authenticate all API requests in this package.
  error_responses:
  - details: Invalid credentials were provided in the request.
    reason: invalid_request
    status: 400
  - details: Missing or expired credentials were provided in the request.
    reason: authentication_failure
    status: 401
  flows:
  - flow: clientCredentials
    scopes: 0
    scopes_note: The spec declares an empty scopes map and the docs name no scopes; access is governed by application approval, not by scope.
    tokenUrl: https://stage.abgapiservices.com/oauth/token/v2
  name: ABG-Access-Token
  sources:
  - openapi/avis-budget-rental-cars-openapi.yml
  - https://developer.avis.com/getting-started
  token_request:
    docs: https://developer.avis.com/getting-started#step-3-get-an-access-token
    headers:
    - client_id
    - client_secret
    method: GET
    url: https://stage.abgapiservices.com/oauth/token/v2
  token_response:
    documented_expires_in_seconds: 7140
    fields:
    - access_token
    - token_type
    - expires_in
    token_type: Bearer
  type: oauth2
slug: avis-budget-authentication
source_filename: avis-budget-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://developer.avis.com/getting-started\ndocs: https://developer.avis.com/getting-started\nspec: openapi/avis-budget-rental-cars-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  note: >-\n    One scheme, OAuth 2.0 client credentials. The Getting Started page documents the exact exchange: a\n    request to https://stage.abgapiservices.com/oauth/token/v2 carrying the application's Client ID and\n    Client Secret as `client_id` / `client_secret` REQUEST HEADERS (the docs' own cURL uses GET, not a\n    form-encoded POST as RFC 6749 §4.4 would), returning {access_token, token_type: Bearer, expires_in}\n    with a documented example expiry of 7140 seconds. Every API call then sends BOTH\n    `Authorization: Bearer <token>` AND the `client_id` header (the spec declares `client_id` as a\n    required header parameter on every operation). Credentials are issued per Client Application after\n\
  \    ABG approval; sandbox/staging credentials are separate from production credentials.\nschemes:\n- name: ABG-Access-Token\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://stage.abgapiservices.com/oauth/token/v2\n    scopes: 0\n    scopes_note: The spec declares an empty scopes map and the docs name no scopes; access is governed by application approval, not by scope.\n  description: OAuth 2.0 client credentials flow used to authenticate all API requests in this package.\n  token_request:\n    method: GET\n    url: https://stage.abgapiservices.com/oauth/token/v2\n    headers: [client_id, client_secret]\n    docs: https://developer.avis.com/getting-started#step-3-get-an-access-token\n  token_response:\n    fields: [access_token, token_type, expires_in]\n    token_type: Bearer\n    documented_expires_in_seconds: 7140\n  api_request_headers:\n    - name: Authorization\n      value: Bearer <access_token>\n    - name: client_id\n      value: <client_id>\n     \
  \ note: Declared as a required header parameter on all 9 operations in the OpenAPI.\n  error_responses:\n    - status: 400\n      reason: invalid_request\n      details: Invalid credentials were provided in the request.\n    - status: 401\n      reason: authentication_failure\n      details: Missing or expired credentials were provided in the request.\n  sources:\n  - openapi/avis-budget-rental-cars-openapi.yml\n  - https://developer.avis.com/getting-started\nonboarding:\n  steps:\n    - Sign up for a portal account at https://developer.avis.com/register (email confirmation, then ABG review — typically 1-2 business days).\n    - Create a Client Application against the Rental Cars API (\"Use this API\" > \"+ New application\"); the Client Secret is shown once.\n    - ABG administrator approves the application; approval email confirms it is ready.\n    - Exchange Client ID/Secret for a Bearer access token; call the API with the token and client_id header.\n    - Contact ABG to launch in\
  \ production; production credentials are separate.\n  self_serve: false\n  approval_required: true\n  docs: https://developer.avis.com/getting-started\nobserved:\n  - url: https://stage.abgapiservices.com/cars/locations/v2/keyword?keyword=Boston\n    status: 401\n    checked: '2026-09-18'\n    www_authenticate: Bearer realm=\"abg-api-preprod.oktapreview.com\", error=\"invalid_token\"\n    body: '{\"error_description\":\"token not found, expired or invalid\",\"error\":\"invalid_grant\"}'\n    note: >-\n      An unauthenticated call is rejected at the gateway with a WWW-Authenticate realm naming an Okta\n      tenant (abg-api-preprod.oktapreview.com), which serves standard OIDC/OAuth discovery documents\n      (recorded in well-known/). The documented token endpoint remains the gateway-fronted\n      /oauth/token/v2, not Okta's /oauth2/v1/token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/authentication/avis-budget-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 500
- Car Rental
- Travel
- Mobility
- Fleet Management
- Transportation
- Reservations
- Vehicle Rental
- Partner API
- Hospitality
---
