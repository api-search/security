---
api_key_in: []
api_specs:
- filename: famous-spring-api-swagger.json
  format: json
  label: Spring Seller API
  slug: spring-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/famous/refs/heads/main/openapi/famous-spring-api-swagger.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Famous Authentication
name_suffix: Authentication
oauth_flows: []
overview: Famous declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Famous
provider_slug: famous
scheme_count: 2
schemes:
- description: 'Seller-scoped bearer credential passed as a URL query parameter (and as formData on POST /seller/v1/messages/send). Every `seller/v1/*` operation declares it `required: true` with the description "authentication token obtained from the V1 Auth API".'
  id: access_token
  in: query
  issued_by: POST /v1/auth-tokens
  lifetime: 24 hours
  lifetime_source: '"The token will expire after 24 hours and require a new request." (POST /v1/auth-tokens description, https://api.teespring.com/swagger_doc/)'
  name: access_token
  reissue: '"you can request a token as often as you want (it will always give you the current one)" — the endpoint returns the CURRENT token rather than minting a new one per call.'
  revocation: not documented
  rotation: not documented
  scope: seller
  transport: query parameter
  type: apiKey
- description: Application identifier issued by Spring/Teespring out of band. Required on the public storefront reads (`GET /v1/campaigns/{slug}`) and required as formData on POST /v1/auth-tokens alongside the account email and password.
  id: app_id
  in: query
  issued_by: manual — "Obtain an app_id from Teespring." (docs page, step 1)
  name: app_id
  scope: application
  self_service: false
  self_service_note: No developer console, key page, or self-serve credential issuance was found on api.teespring.com, spri.ng, amazecommerce.com or amaze.co. An agent has no anonymous path to an app_id; a human must request one from Spring.
  type: apiKey
slug: famous-authentication
source_filename: famous-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.teespring.com/docs\ndocs: https://api.teespring.com/docs\nnote: >-\n  The published Swagger 2.0 document at https://api.teespring.com/swagger_doc/ declares NO\n  `securityDefinitions` block, so `derive-authentication.py` produced nothing. This profile is\n  SEARCHED from the prose and per-operation parameters on the Spring API docs page, which document\n  the scheme explicitly. Nothing here is invented — every value below is quoted or read from a\n  parameter description in the live spec.\napi: Spring Seller API\nbase_url: https://api.teespring.com/\nschemes:\n- id: access_token\n  type: apiKey\n  in: query\n  name: access_token\n  scope: seller\n  description: >-\n    Seller-scoped bearer credential passed as a URL query parameter (and as formData on POST\n    /seller/v1/messages/send). Every `seller/v1/*` operation declares it `required: true` with the\n    description \"authentication token obtained from the\
  \ V1 Auth API\".\n  issued_by: POST /v1/auth-tokens\n  transport: query parameter\n  lifetime: 24 hours\n  lifetime_source: >-\n    \"The token will expire after 24 hours and require a new request.\" (POST /v1/auth-tokens\n    description, https://api.teespring.com/swagger_doc/)\n  reissue: >-\n    \"you can request a token as often as you want (it will always give you the current one)\" —\n    the endpoint returns the CURRENT token rather than minting a new one per call.\n  rotation: not documented\n  revocation: not documented\n- id: app_id\n  type: apiKey\n  in: query\n  name: app_id\n  scope: application\n  description: >-\n    Application identifier issued by Spring/Teespring out of band. Required on the public\n    storefront reads (`GET /v1/campaigns/{slug}`) and required as formData on POST /v1/auth-tokens\n    alongside the account email and password.\n  issued_by: manual — \"Obtain an app_id from Teespring.\" (docs page, step 1)\n  self_service: false\n  self_service_note: >-\n\
  \    No developer console, key page, or self-serve credential issuance was found on\n    api.teespring.com, spri.ng, amazecommerce.com or amaze.co. An agent has no anonymous path to\n    an app_id; a human must request one from Spring.\ntoken_flow:\n  steps:\n  - Obtain an app_id from Teespring.\n  - POST /v1/auth-tokens with formData app_id, email, password (the account's Spring/Teespring\n    login credentials).\n  - Read the access_token from the 201 response body.\n  - Send access_token as a query parameter on every subsequent seller request.\n  verbatim_docs: >-\n    \"1. Obtain an app_id from Teespring. 2. Use the /v1/auth-tokens API endpoint with your email,\n    password, and the provided app_id. 3. Take the token from the response. This is your\n    access_token for future requests. It will last one day, and then you'll need a new one,\n    although you can request a token as often as you want (it will always give you the current\n    one). 4. Make sure your requests always have\
  \ access_token set. Always use https for security!\"\n  grant_type: resource owner password credentials (custom, non-OAuth2 endpoint)\n  response_status: 201\n  response_description: 'Logs in a user and returns an OAuth token'\nobservations:\n  probed: '2026-08-13'\n  unauthenticated_reads:\n  - url: https://api.teespring.com/v1/search-suggestions/trending\n    status: 200\n    note: Returns real data with no credential at all — the only fully anonymous operation observed.\n  missing_credential_behavior:\n  - url: https://api.teespring.com/seller/v1/summary\n    status: 400\n    body: '{\"error\":\"access_token is missing, period is missing\"}'\n  - url: https://api.teespring.com/v1/campaigns/12345\n    status: 400\n    body: '{\"error\":{\"message\":\"app_id is missing\"}}'\ngaps:\n- No OAuth 2.0 authorization server, no OpenID Connect discovery, and no\n  /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource on any Amaze or\n  Spring host (all probed 2026-08-13,\
  \ all 404/301 — see well-known/famous-well-known.yml).\n- No scopes. The access_token is all-or-nothing over the seller's account; there is no way to mint\n  a read-only or campaign-only credential.\n- Credentials are sent in the URL query string rather than an Authorization header, so tokens land\n  in proxy logs, browser history and Referer headers.\n- The token exchange requires the account PASSWORD, so any integration must hold the seller's\n  primary login credential rather than a revocable API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/famous/refs/heads/main/authentication/famous-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Creator Economy
- Commerce
- Live Shopping
- Media
- E-Commerce
- Marketing
- Print on Demand
- Merchandise
- Storefronts
- Order
- Payouts
---
