---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Green Dot Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Green Dot Corporation secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Green Dot Corporation
provider_slug: green-dot
scheme_count: 2
schemes:
- client_authentication: basic
  example_scopes:
  - general
  - demo
  flow: clientCredentials
  grant_type: client_credentials
  name: oauth2ClientCredentials
  scope_optional: true
  scope_style: space-delimited
  sources:
  - docs
  token_endpoint: '{BaasUrl}/authentication'
  token_ttl_seconds: 86400
  token_type: Bearer
  type: oauth2
- applied_to: all protected BaaS endpoints
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
slug: green-dot-authentication
source_filename: green-dot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.greendot.com/embedded-finance/docs/baas-api-authentication\ndocs: https://developer.greendot.com/embedded-finance/docs/baas-api-authentication\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  notes: >-\n    Machine-to-machine OAuth 2.0. Client obtains a Bearer access token from the\n    token endpoint using HTTP Basic (Base64 ClientId:ClientSecret) with\n    grant_type=client_credentials, then presents it as Authorization: Bearer on\n    every call. Tokens are valid 24h (expires_in 86400); recommended cache 23h.\n    IP allow-listing of partner ranges is required before access is granted.\n    Credentials are provisioned per-partner during commercial onboarding.\nschemes:\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: '{BaasUrl}/authentication'\n    grant_type: client_credentials\n    client_authentication:\
  \ basic\n    token_type: Bearer\n    token_ttl_seconds: 86400\n    scope_style: space-delimited\n    scope_optional: true\n    example_scopes: [general, demo]\n    sources: [docs]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    applied_to: all protected BaaS endpoints\n    sources: [docs]\nrequired_headers:\n  - name: Authorization\n    value: 'Bearer <access_token> (or Basic <base64 clientId:clientSecret> on token request)'\n  - name: X-GD-RequestId\n    value: New GUID per call, required for tracing and idempotency\n  - name: Content-Type\n    value: application/json\nauth_errors:\n  - {status: 401, reason: Incorrect credentials or unauthorized scope}\n  - {status: 401, reason: Expired authorization token}\n  - {status: 401, reason: Out of credential scopes}\n  - {status: 400, reason: Malformed request or wrong grant_type}\nconstraints:\n  ip_allowlisting_required: true\n  field_level_encryption: true\n  onboarding: contact-sales\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-dot/refs/heads/main/authentication/green-dot-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Fintech
- Banking as a Service
- Embedded Finance
- Prepaid Cards
- Banking
- Payments
- Money Movement
- United States
---
