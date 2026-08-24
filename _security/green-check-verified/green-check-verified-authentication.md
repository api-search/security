---
api_key_in:
- header
api_specs:
- filename: green-check-verified-access-openapi.yaml
  format: yaml
  label: Green Check Access
  slug: green-check-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-check-verified/refs/heads/main/openapi/green-check-verified-access-openapi.yaml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Green Check Verified Authentication
name_suffix: Authentication
oauth_flows: []
overview: Green Check Verified secures its APIs with oauth2 and apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Green Check Verified
provider_slug: green-check-verified
scheme_count: 1
schemes:
- effective_type: oauth2_client_credentials
  gateway: aws-apigateway custom request authorizer (x-amazon-apigateway-authorizer)
  in: header
  name: access_auth
  parameter: Authorization
  scope_count: 10
  scoped: true
  sources:
  - openapi/green-check-verified-access-openapi.yaml
  - https://developer.greencheckverified.com/guides/integration-overview
  type: apiKey
  value_format: Bearer <access_token>
slug: green-check-verified-authentication
source_filename: green-check-verified-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: >-\n  https://developer.greencheckverified.com/guides/integration-overview +\n  https://developer.greencheckverified.com/tutorials/api-integration-workflow +\n  https://developer.greencheckverified.com/guides/create-crb-connect-pos +\n  openapi/green-check-verified-access-openapi.yaml + live probe of\n  https://prod-api.greencheckverified.com/auth/token (2026-08-22)\ndocs: https://developer.greencheckverified.com/guides/integration-overview\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    One scheme, described two ways. The docs describe OAuth 2.0 client credentials: POST /auth/token\n    with client_id + client_secret + grant_type, returning a Bearer access_token, a scope array and an\n    expires_at timestamp, valid 3600 seconds. The OpenAPI models the same thing as an apiKey scheme\n    named `access_auth` carried in the Authorization header, backed by an AWS API Gateway custom\n \
  \   Lambda authorizer. Per-operation scope requirements ARE declared in the spec under that scheme.\nschemes:\n- name: access_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Bearer <access_token>'\n  effective_type: oauth2_client_credentials\n  scoped: true\n  scope_count: 10\n  gateway: aws-apigateway custom request authorizer (x-amazon-apigateway-authorizer)\n  sources:\n  - openapi/green-check-verified-access-openapi.yaml\n  - https://developer.greencheckverified.com/guides/integration-overview\ntoken_endpoint:\n  operationId: get-token\n  method: POST\n  path: /auth/token\n  security: []\n  unauthenticated: true\n  production: https://prod-api.greencheckverified.com/auth/token\n  sandbox: https://sandbox-api.greencheckverified.com/auth/token\n  request:\n    content_type: application/json\n    fields: [client_id, client_secret, grant_type]\n    grant_type: client_credentials\n  response:\n    fields: [access_token, token_type, scope, expires_at, issued_at,\
  \ client_id]\n    token_type: Bearer\n    lifetime_seconds: 3600\n  probed:\n    date: '2026-08-22'\n    request: 'POST /auth/token with an empty JSON body'\n    status: 422\n    body: '{\"message\":\"Validation Failed\",\"details\":{\"body.client_id\":{\"message\":\"''client_id'' is required\"},\"body.client_secret\":{...},\"body.grant_type\":{...}}}'\n    note: Confirms the endpoint is live, unauthenticated, and validates the three documented fields.\ncredential_issuance:\n  path: >-\n    client_id and client_secret are issued to a service provider by Green Check during commercial\n    onboarding — the docs' \"Choosing Your CRB Onboarding Path\" guide begins \"At this point you have\n    your contract signed, your API credentials, and access to the Green Check web UI.\" There is no\n    self-service key generation; a signed contract precedes access.\n  delegated_credentials:\n    operationId: generate-crb-access-creds\n    path: POST /service-providers/{sp_id}/crbs/{crb_id}/access\n\
  \    description: >-\n      A service provider can mint Green Check Access credentials on behalf of a connected CRB, to\n      operate that CRB's document-management calls. No revoke or rotate operation is published.\ntoken_handling_guidance:\n  - Tokens expire 3600 seconds after issue; check expires_at (unix) and re-authenticate before it passes.\n  - The docs warn that missing refresh logic produces unexpected 401s in production.\n  - client_secret must never be exposed in client-side code (stated in the tutorial).\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-check-verified/refs/heads/main/authentication/green-check-verified-authentication.yml
summary_line: oauth2/apiKey · 1 scheme
tags:
- Company
- Cannabis
- Compliance
- Banking
- Financial Services
- BSA/AML
- Regulatory Technology
- Point of Sale
- Onboarding
- Due Diligence
- Know Your Customer
- Data Aggregation
---
