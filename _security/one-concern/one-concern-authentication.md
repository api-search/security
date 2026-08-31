---
api_key_in: []
api_specs:
- filename: one-concern-location-api-openapi.yml
  format: yaml
  label: One Concern Location API
  slug: one-concern-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-concern/refs/heads/main/openapi/one-concern-location-api-openapi.yml
auth_types: []
description: 'The Domino AI API uses key-based authentication with a customer-issued token carried in a vendor-specific request header. There is no OAuth 2.0, no OpenID Connect, no mTLS and no self-service credential issuance: tokens are obtained by contacting One Concern customer success. A second header, client-id, is required on every call and is used for billing attribution rather than authentication. IMPORTANT PROVENANCE NOTE: the published OpenAPI (openapi/one-concern-domino-ai-openapi.json, Domino AI API v1.31.2) declares NO components.securitySchemes and NO security requirement on any operation, so the derive-from-spec path yields nothing. Everything below is read from the provider''s own documentation prose and confirmed against a live unauthenticated request.'
kind: authentication
layout: security
method: searched
name: One Concern Authentication
name_suffix: Authentication
oauth_flows: []
overview: One Concern declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: One Concern
provider_slug: one-concern
scheme_count: 3
schemes:
- declared_in_openapi: false
  description: Customer-issued API token. One Concern states that a given token may authorize only a subset of the endpoints in the spec, so the published contract describes the full product surface rather than any one customer's entitlement.
  id: api-token
  in: header
  issuance: Manual. "API tokens can be obtained by contacting the One Concern customer success team." No sign-up, developer console, or self-service key page exists.
  name: x-1c-api-token
  required: true
  rotation: not documented
  scopes: none — the API has no scope surface
  type: apiKey
- declared_in_openapi: true
  description: Required on every operation and declared in the OpenAPI as a required header parameter on all five operations. Not a credential — the value "can be anything meaningful to each customer" and is used so One Concern can break down API call volume by group for billing.
  id: client-id
  in: header
  name: client-id
  required: true
  type: apiKey
- declared_in_openapi: true
  description: Optional per-call tracing identifier chosen by the caller; returned in One Concern billing reports on request. Declared in the OpenAPI as an optional header parameter.
  id: transaction-id
  in: header
  name: transaction-id
  required: false
  type: apiKey
slug: one-concern-authentication
source_filename: one-concern-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developer.oneconcern.com/overview\ndocs: https://developer.oneconcern.com/overview\nname: One Concern Domino AI API Authentication\ndescription: >-\n  The Domino AI API uses key-based authentication with a customer-issued token carried in a\n  vendor-specific request header. There is no OAuth 2.0, no OpenID Connect, no mTLS and no\n  self-service credential issuance: tokens are obtained by contacting One Concern customer\n  success. A second header, client-id, is required on every call and is used for billing\n  attribution rather than authentication.\n  IMPORTANT PROVENANCE NOTE: the published OpenAPI (openapi/one-concern-domino-ai-openapi.json,\n  Domino AI API v1.31.2) declares NO components.securitySchemes and NO security requirement on\n  any operation, so the derive-from-spec path yields nothing. Everything below is read from the\n  provider's own documentation prose and confirmed against a live unauthenticated\
  \ request.\nschemes:\n- id: api-token\n  type: apiKey\n  in: header\n  name: x-1c-api-token\n  required: true\n  description: >-\n    Customer-issued API token. One Concern states that a given token may authorize only a\n    subset of the endpoints in the spec, so the published contract describes the full product\n    surface rather than any one customer's entitlement.\n  issuance: >-\n    Manual. \"API tokens can be obtained by contacting the One Concern customer success team.\"\n    No sign-up, developer console, or self-service key page exists.\n  rotation: not documented\n  scopes: none — the API has no scope surface\n  declared_in_openapi: false\n- id: client-id\n  type: apiKey\n  in: header\n  name: client-id\n  required: true\n  description: >-\n    Required on every operation and declared in the OpenAPI as a required header parameter on\n    all five operations. Not a credential — the value \"can be anything meaningful to each\n    customer\" and is used so One Concern can break\
  \ down API call volume by group for billing.\n  declared_in_openapi: true\n- id: transaction-id\n  type: apiKey\n  in: header\n  name: transaction-id\n  required: false\n  description: >-\n    Optional per-call tracing identifier chosen by the caller; returned in One Concern billing\n    reports on request. Declared in the OpenAPI as an optional header parameter.\n  declared_in_openapi: true\ntransport:\n  https_required: true\n  note: >-\n    \"All API requests must be made over HTTPS. Calls made over plain HTTP will fail.\" Confirmed:\n    api.oneconcern.com serves HTTP/2 over TLSv1.3.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nsigned_requests: false\nverification:\n  method: probed\n  fetched: '2026-08-26'\n  request: >-\n    POST https://api.oneconcern.com/v1/location/business-interruption/return-period with\n    client-id and a JSON body, no x-1c-api-token\n  http_status: 401\n  response_body: '{\"error\": \"Authorization field missing\"}'\n  gateway: 'x-generator:\
  \ tyk.io'\n  note: >-\n    An undocumented path on the same host returns 404, so the 401 confirms both that\n    api.oneconcern.com is the real base URL for this contract and that the documented auth\n    model is enforced at the gateway.\ngaps:\n- The OpenAPI declares no securitySchemes, so a generated client or an agent reading only the\n  spec cannot discover that x-1c-api-token is required. Adding an apiKey scheme and a global\n  security requirement would be a one-line fix with a large agent-readability payoff.\n- No documented token rotation, expiry, or revocation procedure.\n- No self-service credential path; every integration begins with a sales conversation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-concern/refs/heads/main/authentication/one-concern-authentication.yml
summary_line: 3 schemes
tags:
- Climate Risk
- Catastrophe Modeling
- Resilience
- Insurance
- Reinsurance
- Risk Analytics
- Geospatial
- Business Interruption
- Real-Estate
- Financial-Services
- Artificial Intelligence
---
