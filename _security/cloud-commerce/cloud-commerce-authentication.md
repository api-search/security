---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Cloud Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Commerce declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud Commerce
provider_slug: cloud-commerce
scheme_count: 1
schemes:
- confidence: medium
  credentials:
  - evidence: POST {} returned 400 with data.error.email = ["The email field is required."]
    field: email
    required: true
  - evidence: POST {} returned 400 with data.error.password = ["The password field is required."]
    field: password
    required: true
  grant: password
  id: login_token
  note: The endpoint's own 400 body states its purpose is "For logged in and generate Token." A bad-credential POST returns 401 with "Email or Password incorrect." The response header name that carries the issued token, its lifetime, its refresh mechanism and the header an authenticated call must send are NOT public and were NOT probed — issuing a token would require real credentials, which this pipeline never uses.
  observed: true
  purpose_stated_by_provider: For logged in and generate Token.
  style: bearer-token-via-credential-exchange
  token_endpoint: https://openapi.fastship.co/api/v2/login
  token_endpoint_methods:
  - GET
  - HEAD
  - POST
  type: http
slug: cloud-commerce-authentication
source_filename: cloud-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://openapi.fastship.co/api/v2/login\nnote: PROBED, NOT DERIVED. Cloud Commerce publishes no OpenAPI and no public authentication reference, so derive-authentication.py\n  had nothing to read. This profile is built entirely from anonymous live requests against the FastShip Open API host, and\n  records only what those responses actually proved. No scheme, header name, token lifetime or scope is asserted that was\n  not observed.\napis:\n- name: FastShip Open API\n  baseURL: https://openapi.fastship.co/api/v2\n  schemes:\n  - &id001\n    id: login_token\n    type: http\n    style: bearer-token-via-credential-exchange\n    confidence: medium\n    observed: true\n    token_endpoint: https://openapi.fastship.co/api/v2/login\n    token_endpoint_methods:\n    - GET\n    - HEAD\n    - POST\n    grant: password\n    credentials:\n    - field: email\n      required: true\n      evidence: POST {} returned 400 with data.error.email\
  \ = [\"The email field is required.\"]\n    - field: password\n      required: true\n      evidence: POST {} returned 400 with data.error.password = [\"The password field is required.\"]\n    purpose_stated_by_provider: For logged in and generate Token.\n    note: The endpoint's own 400 body states its purpose is \"For logged in and generate Token.\" A bad-credential POST returns\n      401 with \"Email or Password incorrect.\" The response header name that carries the issued token, its lifetime, its refresh\n      mechanism and the header an authenticated call must send are NOT public and were NOT probed — issuing a token would\n      require real credentials, which this pipeline never uses.\nevidence:\n- url: https://openapi.fastship.co/api/v2\n  method: GET\n  status: 200\n  body: Welcome to API Version 2.0\n- url: https://openapi.fastship.co/api/v2/login\n  method: GET\n  status: 401\n  body: '{\"message\":\"failed\",\"description\":\"Login failed\",\"data\":[]}'\n- url: https://openapi.fastship.co/api/v2/login\n\
  \  method: POST\n  status: 400\n  note: empty JSON body; returned per-field validation errors for email and password\n- url: https://openapi.fastship.co/api/v2/login\n  method: POST\n  status: 401\n  note: syntactically valid but non-existent credentials; \"Email or Password incorrect.\"\n- url: https://openapi.fastship.co/api/v2/login\n  method: OPTIONS\n  status: 200\n  allow: GET,HEAD,POST\ngaps:\n- no OpenAPI or Swagger document is published on any Cloud Commerce host\n- no public authentication reference page\n- no /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host, so this is not an OAuth or\n  OIDC surface\n- 'the authenticated request header (Authorization: Bearer vs a custom header) is undocumented and unverifiable without credentials'\nschemes:\n- *id001\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-commerce/refs/heads/main/authentication/cloud-commerce-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-Commerce
- Logistics
- Marketplace
- Influencer Marketing
- Cross-Border Commerce
- Small Business
- Southeast Asia
- Shipping
- Fulfillment
- Thailand
---
