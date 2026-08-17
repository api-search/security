---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Cloud Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Commerce declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud Commerce
provider_slug: cloud-commerce
scheme_count: 0
schemes: []
slug: cloud-commerce-authentication
source_filename: cloud-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://openapi.fastship.co/api/v2/login\nnote: >-\n  PROBED, NOT DERIVED. Cloud Commerce publishes no OpenAPI and no public authentication\n  reference, so derive-authentication.py had nothing to read. This profile is built\n  entirely from anonymous live requests against the FastShip Open API host, and records\n  only what those responses actually proved. No scheme, header name, token lifetime or\n  scope is asserted that was not observed.\napis:\n- name: FastShip Open API\n  baseURL: https://openapi.fastship.co/api/v2\n  schemes:\n  - id: login_token\n    type: http\n    style: bearer-token-via-credential-exchange\n    confidence: medium\n    observed: true\n    token_endpoint: https://openapi.fastship.co/api/v2/login\n    token_endpoint_methods:\n    - GET\n    - HEAD\n    - POST\n    grant: password\n    credentials:\n    - field: email\n      required: true\n      evidence: >-\n        POST {} returned 400 with data.error.email\
  \ = [\"The email field is required.\"]\n    - field: password\n      required: true\n      evidence: >-\n        POST {} returned 400 with data.error.password = [\"The password field is required.\"]\n    purpose_stated_by_provider: For logged in and generate Token.\n    note: >-\n      The endpoint's own 400 body states its purpose is \"For logged in and generate\n      Token.\" A bad-credential POST returns 401 with \"Email or Password incorrect.\"\n      The response header name that carries the issued token, its lifetime, its refresh\n      mechanism and the header an authenticated call must send are NOT public and were\n      NOT probed — issuing a token would require real credentials, which this pipeline\n      never uses.\nevidence:\n- url: https://openapi.fastship.co/api/v2\n  method: GET\n  status: 200\n  body: Welcome to API Version 2.0\n- url: https://openapi.fastship.co/api/v2/login\n  method: GET\n  status: 401\n  body: '{\"message\":\"failed\",\"description\":\"Login failed\"\
  ,\"data\":[]}'\n- url: https://openapi.fastship.co/api/v2/login\n  method: POST\n  status: 400\n  note: empty JSON body; returned per-field validation errors for email and password\n- url: https://openapi.fastship.co/api/v2/login\n  method: POST\n  status: 401\n  note: syntactically valid but non-existent credentials; \"Email or Password incorrect.\"\n- url: https://openapi.fastship.co/api/v2/login\n  method: OPTIONS\n  status: 200\n  allow: GET,HEAD,POST\ngaps:\n- no OpenAPI or Swagger document is published on any Cloud Commerce host\n- no public authentication reference page\n- >-\n  no /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any\n  host, so this is not an OAuth or OIDC surface\n- >-\n  the authenticated request header (Authorization: Bearer vs a custom header) is\n  undocumented and unverifiable without credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-commerce/refs/heads/main/authentication/cloud-commerce-authentication.yml
summary_line: 0 schemes
tags:
- Company
- E-Commerce
- Logistics
- Marketplace
- Influencer Marketing
- Cross-Border Commerce
- SME
- Southeast Asia
- Shipping
- Fulfillment
- Thailand
---
