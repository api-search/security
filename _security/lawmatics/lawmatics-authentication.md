---
api_key_in: []
api_specs:
- filename: lawmatics-openapi.yml
  format: yaml
  label: Lawmatics OAuth API
  slug: lawmatics-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawmatics/refs/heads/main/openapi/lawmatics-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lawmatics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lawmatics secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lawmatics
provider_slug: lawmatics
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization code grant. Register a developer app at https://app.lawmatics.com/settings/developers (developer settings must be enabled by Lawmatics support). Access tokens are non-expiring; no refresh tokens are issued and scopes are not supported.
  flows:
  - authorizationUrl: https://app.lawmatics.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.lawmatics.com/oauth/token
  name: oauth2
  sources:
  - openapi/lawmatics-openapi.yml
  type: oauth2
- description: 'The OAuth 2.0 access token is sent as `Authorization: Bearer <access_token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lawmatics-openapi.yml
  type: http
slug: lawmatics-authentication
source_filename: lawmatics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.lawmatics.com/\ndocs: https://docs.lawmatics.com/\ndocs_detail: The \"Getting Started With Auth\" section of the Lawmatics-published Postman documentation,\n  plus https://help.lawmatics.com/en/articles/10699983-lawmatics-open-api\nderived_from: openapi/lawmatics-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.lawmatics.com/oauth/authorize\n    tokenUrl: https://api.lawmatics.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authorization code grant. Register a developer app at https://app.lawmatics.com/settings/developers\n    (developer settings must be enabled by Lawmatics support). Access tokens are non-expiring; no refresh\n    tokens are issued and scopes are not supported.\n  sources:\n  - openapi/lawmatics-openapi.yml\n- name: bearerAuth\n\
  \  type: http\n  scheme: bearer\n  description: 'The OAuth 2.0 access token is sent as `Authorization: Bearer <access_token>`.'\n  sources:\n  - openapi/lawmatics-openapi.yml\nonboarding:\n  self_service: false\n  gate: Developer settings must be enabled on the account by a Lawmatics support representative before\n    a developer app can be created.\n  app_registration_url: https://app.lawmatics.com/settings/developers\n  required_app_fields:\n  - Name\n  - Description\n  - Logo\n  - Callback URL\nflow:\n  step_1: Redirect the user to https://app.lawmatics.com/oauth/authorize with client_id, redirect_uri,\n    response_type=code and an optional state.\n  step_2: Lawmatics redirects back to redirect_uri with a short-lived ?code= grant token.\n  step_3: POST https://api.lawmatics.com/oauth/token from your backend with client_id, client_secret,\n    grant_type=authorization_code, code and redirect_uri.\n  step_4: 'The response is {\"token_type\":\"bearer\",\"access_token\":\"...\",\"created_at\"\
  :<unix>}. Send it as\n    Authorization: Bearer <access_token>.'\ntoken_properties:\n  expires: false\n  refresh_token: false\n  scopes: false\n  revocation_endpoint: false\n  grants: full CRUD over the authorizing firm account\n  note: 'Lawmatics states all four directly: \"We currently do not support scopes. Once a user authenticates\n    your app, they are giving you full CRUD access to their account\", \"We do not have a deauthorization\n    endpoint\", and \"We do not give you a refresh token. Access tokens do not expire so they are not needed.\"\n    A leaked Lawmatics access token is a permanent, unscoped, unrevocable key to a law firm''s client\n    data.'\nunauthenticated_operations:\n- operation: submitCustomFormEntryFormDataBody\n  path: POST /v1/forms/{custom_form_uuid}/submit\n  note: Public custom-form submission; marked noauth in the published collection. The form UUID is the\n    only credential.\ndiscovery:\n  oauth_authorization_server_metadata: false\n  openid_configuration:\
  \ false\n  note: Neither RFC 8414 nor OIDC discovery documents are served; see well-known/lawmatics-well-known.yml\nevidence:\n- url: https://api.lawmatics.com/v1/contacts\n  method: GET\n  http_status: 401\n  checked: '2026-08-13'\n  note: unauthenticated request rejected, confirming the bearer requirement\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawmatics/refs/heads/main/authentication/lawmatics-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Legal
- CRM
- Law Firms
- Client Intake
- Marketing Automation
- Matter Management
- E-Signature
- Workflow Automation
- Legal Tech
- Time and Billing
- Webhooks
- OAuth
---
