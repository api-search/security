---
api_key_in: []
api_specs:
- filename: autofi-api-openapi.yml
  format: yaml
  label: AutoFi API
  slug: autofi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Autofi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoFi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AutoFi
provider_slug: autofi
scheme_count: 1
schemes:
- bearerFormat: Bearer {token}
  description: Get access to data while protecting your account credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/autofi-api-openapi.yml
  type: http
slug: autofi-authentication
source_filename: autofi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/autofi-api-openapi.yml\ndocs: https://api.autofi.com/api.html\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  model: >-\n    JWT bearer. API client credentials (clientId + clientSecret) are exchanged at\n    POST /auth/token for a short-lived JSON Web Token, which is then sent as\n    `Authorization: Bearer {token}` on every other operation. Scope strings are\n    attached to the bearer requirement per operation (see scopes/autofi-scopes.yml).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer {token}\n  description: Get access to data while protecting your account credentials.\n  sources:\n  - openapi/autofi-api-openapi.yml\ntoken_endpoint:\n  operation: POST /auth/token\n  security: none (this operation declares an empty security requirement)\n  request:\n    content_type: application/json\n    required_fields:\n    - clientId\n    - clientSecret\n  response:\n\
  \    fields:\n    - name: access_token\n      description: JSON Web Token format\n    - name: expires_in\n      description: seconds after issuance the token expires in\n      documented_example: 86400\n    - name: token_type\n      documented_example: Bearer\n  errors:\n  - status: 401\n    shape: '{\"error\": \"UnauthorizedError: invalid token\"}'\ncredential_issuance:\n  self_serve: false\n  note: >-\n    The reference does not publish a self-serve path to obtain clientId /\n    clientSecret. API client credentials are issued by AutoFi to dealer, OEM,\n    lender and marketplace partners; the public entry point is the demo/contact\n    form at https://www.autofi.com/request-demo/.\nenvironments:\n- name: Production\n  base_url: https://api.autofi.com\n- name: Test Sandbox (UAT)\n  base_url: https://api-uat.autofi.com\nnotes:\n- >-\n  Documented 401 error bodies use a flat {\"error\": \"UnauthorizedError: ...\"}\n  envelope, which differs from the {code,message,errors[]} envelope used\
  \ for\n  validation errors. See errors/autofi-problem-types.yml.\n- >-\n  No OAuth 2.0 authorization-server metadata is published: /.well-known/\n  oauth-authorization-server and /.well-known/openid-configuration return 404 on\n  api.autofi.com, api-uat.autofi.com and auth.autofi.com (probed 2026-08-14).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/authentication/autofi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Fintech
- Digital Retail
- Auto Finance
- Dealerships
- Sales Enablement
- Software-as-a-Service
- Lending
- Loan Origination
- Credit Decisioning
- Payment Calculation
- Prequalification
---
