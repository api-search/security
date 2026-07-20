---
api_key_in:
- header
api_specs:
- filename: kitchenstories-internal-openapi.json
  format: json
  label: Kitchen Stories Internal API
  slug: internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitchenstories/refs/heads/main/openapi/kitchenstories-internal-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kitchenstories Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kitchen Stories secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kitchen Stories
provider_slug: kitchenstories
scheme_count: 2
schemes:
- applied: global
  bearerFormat: JWT
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/kitchenstories-internal-openapi.json
  type: http
- applied: global
  in: header
  name: ApiKeyAuth
  notes: Vendor-specific user-identity header used alongside or in place of the bearer token; not a self-service API key and not documented publicly.
  parameter: X-Ultron-User
  sources:
  - openapi/kitchenstories-internal-openapi.json
  type: apiKey
slug: kitchenstories-authentication
source_filename: kitchenstories-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  openapi/kitchenstories-internal-openapi.json plus live probes of\n  https://api.kitchenstories.io/api/ on 2026-07-19\ndocs: https://api.kitchenstories.io/api/\nsummary:\n  model: bearer-token\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  scopes: false\n  public_program: false\n  notes: >-\n    The Kitchen Stories Internal API is a first-party backend with no public developer program,\n    no self-service key issuance and no OAuth 2.0 authorization server. Credentials are minted by\n    the API's own /authenticate/ endpoints, which return a JWT bearer token that is presented on\n    every subsequent call. Security is declared globally in the spec (top-level `security`), so\n    all 157 operations require a credential; no operation opts out with an empty security array.\n    Because there is no oauth2 securityScheme and no scope surface, no scopes/ artifact is\n    produced for this provider.\n\
  schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  applied: global\n  sources:\n  - openapi/kitchenstories-internal-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Ultron-User\n  applied: global\n  notes: >-\n    Vendor-specific user-identity header used alongside or in place of the bearer token; not a\n    self-service API key and not documented publicly.\n  sources:\n  - openapi/kitchenstories-internal-openapi.json\nflows:\n- name: email-and-password\n  operationId: autenticate-credentials\n  method: POST\n  path: /authenticate/credentials/\n  returns: access_token\n- name: anonymous-or-device\n  operationId: autenticate\n  method: POST\n  path: /authenticate/\n  returns: access_token\n- name: sign-in-with-apple\n  operationId: autenticate-appleid\n  method: POST\n  path: /authenticate/appleid/\n  returns: access_token\n- name: google\n  operationId: autenticate-google\n  method:\
  \ POST\n  path: /authenticate/google/\n  returns: access_token\n- name: facebook\n  operationId: autenticate-facebook\n  method: POST\n  path: /authenticate/facebook/\n  returns: access_token\nregistration:\n- operationId: register-credentials\n  method: POST\n  path: /register/\n  description: Create a new user with email and password.\n- operationId: validate-email\n  method: GET\n  path: /users/validate/email\n  description: Validate the email link generated on account creation (no trailing slash).\n- operationId: password-forgot\n  method: POST\n  path: /password/forgot/\n- operationId: password-reset\n  method: GET\n  path: /password/reset/\nobserved:\n  unauthenticated_request:\n    url: https://api.kitchenstories.io/api/recipes/{slug}/\n    status: 401\n    www_authenticate: Bearer\n    content_type: application/vnd.ajns.kitchenstories+json\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitchenstories/refs/heads/main/authentication/kitchenstories-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Food and Beverage
- Recipes
- Cooking
- Media
- Content
- Consumer
- Mobile
- Video
- Germany
---
