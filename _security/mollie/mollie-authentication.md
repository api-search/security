---
api_key_in:
- header
api_specs:
- filename: mollie-openapi-original.yml
  format: yaml
  label: Mollie API
  slug: mollie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/openapi/mollie-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mollie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mollie secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mollie
provider_slug: mollie
scheme_count: 4
schemes:
- description: Authenticates API requests for a single website profile. Each key targets either live mode (live_...) or test mode (test_...). Keys are shown only once, at creation, and cannot be retrieved afterwards; a lost key must be replaced under Developers → API access tokens in the Dashboard and the old one revoked.
  in: header
  name: apiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/mollie-openapi-original.yml
  token_prefixes:
  - live_
  - test_
  type: http
- description: Authenticates API requests with configurable permissions. Can access organization-level resources and optionally scope to a specific payment profile. Intended for advanced integrations such as bookkeeping or reporting tools that need fine-grained control. Shown only once at creation. Supports the testmode request parameter instead of a separate test key.
  in: header
  name: advancedAccessToken
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/mollie-openapi-original.yml
  token_prefixes:
  - access_
  type: http
- description: Mollie Connect. OAuth 2.0 authorization code flow used by platforms and marketplaces to act on behalf of linked merchant organizations.
  flows:
  - authorizationUrl: https://my.mollie.com/oauth2/authorize
    flow: authorizationCode
    scope_count: 60
    scopes_artifact: scopes/mollie-scopes.yml
    tokenUrl: https://api.mollie.com/oauth2/tokens
  metadata:
    code_challenge_methods_supported:
    - S256
    dynamic_client_registration: true
    grant_types_supported:
    - authorization_code
    - refresh_token
    issuer: https://my.mollie.com
    registration_endpoint: https://api.mollie.com/oauth2/register
    response_types_supported:
    - code
    revocation_endpoint: https://api.mollie.com/oauth2/tokens
    service_documentation: https://docs.mollie.com/reference/oauth2
    token_endpoint_auth_methods_supported:
    - client_secret_post
    - none
  name: oAuth
  sources:
  - openapi/mollie-openapi-original.yml
  - https://my.mollie.com/.well-known/oauth-authorization-server
  type: oauth2
- description: HTTP Basic Authentication, encoded as "Basic " + toBase64(username + ":" + password). Used on the OAuth token endpoints for confidential clients.
  in: header
  name: basicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - openapi/mollie-openapi-original.yml
  type: http
slug: mollie-authentication
source_filename: mollie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/mollie-openapi-original.yml\ndocs: https://docs.mollie.com/reference/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer, basic]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  transport: HTTPS only, Authorization header\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  sources: [openapi/mollie-openapi-original.yml]\n  description: >-\n    Authenticates API requests for a single website profile. Each key targets either\n    live mode (live_...) or test mode (test_...). Keys are shown only once, at creation,\n    and cannot be retrieved afterwards; a lost key must be replaced under Developers →\n    API access tokens in the Dashboard and the old one revoked.\n  token_prefixes: [live_, test_]\n- name: advancedAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  sources: [openapi/mollie-openapi-original.yml]\n\
  \  description: >-\n    Authenticates API requests with configurable permissions. Can access\n    organization-level resources and optionally scope to a specific payment profile.\n    Intended for advanced integrations such as bookkeeping or reporting tools that need\n    fine-grained control. Shown only once at creation. Supports the testmode request\n    parameter instead of a separate test key.\n  token_prefixes: [access_]\n- name: oAuth\n  type: oauth2\n  sources: [openapi/mollie-openapi-original.yml, https://my.mollie.com/.well-known/oauth-authorization-server]\n  description: >-\n    Mollie Connect. OAuth 2.0 authorization code flow used by platforms and marketplaces\n    to act on behalf of linked merchant organizations.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.mollie.com/oauth2/authorize\n    tokenUrl: https://api.mollie.com/oauth2/tokens\n    scope_count: 60\n    scopes_artifact: scopes/mollie-scopes.yml\n  metadata:\n    issuer: https://my.mollie.com\n\
  \    registration_endpoint: https://api.mollie.com/oauth2/register\n    revocation_endpoint: https://api.mollie.com/oauth2/tokens\n    service_documentation: https://docs.mollie.com/reference/oauth2\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_post, none]\n    dynamic_client_registration: true\n- name: basicAuth\n  type: http\n  scheme: basic\n  in: header\n  parameter: Authorization\n  sources: [openapi/mollie-openapi-original.yml]\n  description: >-\n    HTTP Basic Authentication, encoded as \"Basic \" + toBase64(username + \":\" + password).\n    Used on the OAuth token endpoints for confidential clients.\nrequest_signing:\n  present: true\n  scope: Business Account Transfers API (create-transfer)\n  headers: [X-Client-Signature, X-Client-Signed-At]\n  note: >-\n    Transfers from a Mollie Business Account must additionally\
  \ be signed, on top of the\n    bearer advanced access token, and must carry an Idempotency-Key header.\nmcp:\n  url: https://mcp.mollie.com/mcp\n  scheme: bearer\n  minimum_scope: profile.read\n  protected_resource_metadata: https://mcp.mollie.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/authentication/mollie-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Payments
- Fintech
- Financial-Services
- Checkout
- E-Commerce
- Subscription
- Point-of-Sale
- Europe
- Netherlands
---
