---
api_key_in:
- header
api_specs:
- filename: light-openapi-original.json
  format: json
  label: Light API
  slug: light-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/openapi/light-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Light Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Light secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Light
provider_slug: light
scheme_count: 3
schemes:
- authorization_model: API keys are linked to roles the same way user accounts are; the roles assigned to the key determine what actions it can perform.
  description: Basic authentication header of the form "Basic <api_key>", where <api_key> is your API key.
  example: 'Authorization: Basic [example key]'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  provisioning: Log in to Light, navigate to Settings > API Keys and click Create Key. The generated key is shown once and must be stored securely.
  scheme: Basic
  sources:
  - openapi/light-openapi-original.json
  - https://docs.light.inc/getting-started/authentication
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 access token presented as a bearer JWT.
  example: 'Authorization: Bearer [example key]'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/light-openapi-original.json
  - https://docs.light.inc/getting-started/authentication
  type: http
- documented_only: true
  enablement: Contact Light support at help@light.inc to set up your account for the OAuth 2.0 flow. You receive a client_id and client_secret and register a redirect URI.
  flows:
  - authorizationUrl: https://api.light.inc/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    parameters:
    - client_id
    - redirect_uri
    - state
    refreshUrl: https://api.light.inc/oauth/token
    scopes: {}
    scopes_documented: false
    tokenUrl: https://api.light.inc/oauth/token
    token_request_content_type: application/x-www-form-urlencoded
  identity_provider:
    evidence: A live GET to https://api.light.inc/oauth/authorize?client_id=...&redirect_uri=... returns an authorization page whose stylesheets load from cdn.auth0.com, indicating the OAuth authorization surface is backed by Auth0.
    probed: '2026-07-19'
    vendor: Auth0
  name: oauth2
  operations:
  - startOAuthAuthorizationFlow
  - getOAuthToken
  parameter_naming_note: Calling /oauth/authorize with no parameters returns {"type":"MISSING_PARAMETER","message":"Missing parameter 'redirectUri'"} — camelCase — but the documented snake_case redirect_uri is what the endpoint actually accepts (it renders the authorization page). The error message wording does not match the accepted parameter name.
  refresh_token_notes: The refresh response returns a NEW access_token, refresh_token and expires_in. The old refresh token is invalidated after use, so stored refresh tokens must be updated.
  refresh_token_rotation: true
  sources:
  - https://docs.light.inc/getting-started/authentication
  token_response_fields:
  - access_token
  - refresh_token
  - expires_in
  type: oauth2
slug: light-authentication
source_filename: light-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.light.inc/getting-started/authentication\ndocs: https://docs.light.inc/getting-started/authentication\nspec_source: openapi/light-openapi-original.json\nnote: >-\n  Upgraded from derived to searched: the OpenAPI declares only apiKey + bearer, but the\n  documentation publishes a full OAuth 2.0 authorization-code flow (with authorize/token\n  endpoints and refresh-token rotation) that the spec omits.\n\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  transport: HTTPS required — calls made over plain HTTP fail.\n\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme: Basic\n  example: 'Authorization: Basic [example key]'\n  description: >-\n    Basic authentication header of the form \"Basic <api_key>\", where <api_key> is your API key.\n  provisioning: >-\n    Log in to Light, navigate to Settings\
  \ > API Keys and click Create Key. The generated key is\n    shown once and must be stored securely.\n  authorization_model: >-\n    API keys are linked to roles the same way user accounts are; the roles assigned to the key\n    determine what actions it can perform.\n  sources:\n  - openapi/light-openapi-original.json\n  - https://docs.light.inc/getting-started/authentication\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  example: 'Authorization: Bearer [example key]'\n  description: OAuth 2.0 access token presented as a bearer JWT.\n  sources:\n  - openapi/light-openapi-original.json\n  - https://docs.light.inc/getting-started/authentication\n- name: oauth2\n  type: oauth2\n  documented_only: true\n  enablement: >-\n    Contact Light support at help@light.inc to set up your account for the OAuth 2.0 flow.\n    You receive a client_id and client_secret and register a redirect URI.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.light.inc/oauth/authorize\n\
  \    tokenUrl: https://api.light.inc/oauth/token\n    refreshUrl: https://api.light.inc/oauth/token\n    parameters:\n    - client_id\n    - redirect_uri\n    - state\n    token_request_content_type: application/x-www-form-urlencoded\n    grant_types:\n    - authorization_code\n    - refresh_token\n    scopes: {}\n    scopes_documented: false\n  token_response_fields:\n  - access_token\n  - refresh_token\n  - expires_in\n  refresh_token_rotation: true\n  refresh_token_notes: >-\n    The refresh response returns a NEW access_token, refresh_token and expires_in. The old\n    refresh token is invalidated after use, so stored refresh tokens must be updated.\n  operations:\n  - startOAuthAuthorizationFlow\n  - getOAuthToken\n  identity_provider:\n    vendor: Auth0\n    evidence: >-\n      A live GET to https://api.light.inc/oauth/authorize?client_id=...&redirect_uri=... returns\n      an authorization page whose stylesheets load from cdn.auth0.com, indicating the OAuth\n      authorization\
  \ surface is backed by Auth0.\n    probed: '2026-07-19'\n  parameter_naming_note: >-\n    Calling /oauth/authorize with no parameters returns\n    {\"type\":\"MISSING_PARAMETER\",\"message\":\"Missing parameter 'redirectUri'\"} — camelCase — but\n    the documented snake_case redirect_uri is what the endpoint actually accepts (it renders the\n    authorization page). The error message wording does not match the accepted parameter name.\n  sources:\n  - https://docs.light.inc/getting-started/authentication\n\nclient_requirements:\n- Follow HTTP redirects AND forward the Authorization header, as some endpoints redirect to other URLs.\n- Send all requests over HTTPS.\n\nscopes:\n  published: false\n  notes: >-\n    Light documents no OAuth scope surface — access is governed by the roles attached to the\n    API key or user account, not by per-token scopes. No scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/authentication/light-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Accounting
- Finance
- ERP
- Accounts Payable
- Accounts Receivable
- General Ledger
- Spend Management
- Invoicing
- Corporate Cards
- Expense Management
- Financial Operations
- Agents
- Company
---
