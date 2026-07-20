---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kasko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kasko secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kasko
provider_slug: kasko
scheme_count: 2
schemes:
- description: Provide your secret API key as the HTTP Basic auth username value; no password is required. All requests must be made over HTTPS.
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md
  type: http
- description: 'Alternatively (e.g. for cross-origin requests) send the secret API key as a bearer token: Authorization: Bearer [example key]'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md
  type: http
slug: kasko-authentication
source_filename: kasko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md\ndocs: https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  key_model: secret-api-key\n  test_live_separation: true\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Provide your secret API key as the HTTP Basic auth username value; no\n      password is required. All requests must be made over HTTPS.\n    sources: [https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Alternatively (e.g. for cross-origin requests) send the secret API key as\n      a bearer token: Authorization: Bearer [example key]\n    sources: [https://docs.kasko.io/kasko-api-documentation/rest-api/introduction.md]\nkeys:\n  secret_keys:\n    - name: TEST secret\
  \ key\n      prefix: sk_test_\n      purpose: Development; no real insurance policies are created.\n    - name: LIVE secret key\n      prefix: sk_live_\n      purpose: Production; issues real insurance policies and payments are owed by the distributor.\n  client_keys:\n    - name: TEST client key\n      purpose: Front-end (KASKO JS) testing with test credit card credentials; no real charges.\n    - name: LIVE client key\n      purpose: Front-end production; real charges and real policies.\n  product_keys:\n    description: Distinct product key issued per insurance product; supplied to both KASKO JS and the REST API.\nnotes: >-\n  Requests requiring authentication may return 404 Not Found instead of 403\n  Forbidden to avoid leaking existence of sensitive resources. Keys can be\n  rotated by contacting support@kasko.io.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kasko/refs/heads/main/authentication/kasko-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Insurance
- InsurTech
- Insurance API
- Policy Management
- Payments
- Webhooks
- Embedded Insurance
- No-Code
---
