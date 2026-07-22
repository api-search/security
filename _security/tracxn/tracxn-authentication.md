---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Tracxn API
  slug: tracxn-api
  spec_type: Postman
  url: https://www.postman.com/tracxnapi/tracxn-api/overview
auth_types:
- apiKey
description: Authentication profile for the Tracxn API v2.2. Tracxn does not publish a public OpenAPI; the reference documentation sits behind the platform login. The API authenticates every request with an account-scoped access token passed in a lowercase `accesstoken` HTTP header. Tokens are issued from the Tracxn platform under Data Solutions > API & Developer Tools (separate Playground and production tokens). Requests without a token are rejected with a JSON error envelope (errorCode 403000000, "Invalid web session access. No user." observed live on 2026-07-21). No OAuth 2.0, OpenID Connect, or scope surface is documented.
kind: authentication
layout: security
method: searched
name: Tracxn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tracxn secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tracxn
provider_slug: tracxn
scheme_count: 1
schemes:
- environments:
  - production: https://platform.tracxn.com/api/2.2
  - playground: https://platform.tracxn.com/api/2.2/playground
  in: header
  issuance: Tracxn platform > Data Solutions > API & Developer Tools > API Token
  name: accesstoken
  parameter: accesstoken
  type: apiKey
slug: tracxn-authentication
source_filename: tracxn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://w.tracxn.com/api-developers-page ; live probe of\n  https://platform.tracxn.com/api/2.2/companies (403 without token) ;\n  https://www.postman.com/tracxnapi/tracxn-api (official Postman workspace) ;\n  public client implementations of the documented v2.2 contract\ndocs: https://platform.tracxn.com/a/api/gettingstarted/apibasics\ndescription: >-\n  Authentication profile for the Tracxn API v2.2. Tracxn does not publish a\n  public OpenAPI; the reference documentation sits behind the platform login.\n  The API authenticates every request with an account-scoped access token\n  passed in a lowercase `accesstoken` HTTP header. Tokens are issued from the\n  Tracxn platform under Data Solutions > API & Developer Tools (separate\n  Playground and production tokens). Requests without a token are rejected\n  with a JSON error envelope (errorCode 403000000, \"Invalid web session\n  access. No user.\" observed live on 2026-07-21).\
  \ No OAuth 2.0, OpenID\n  Connect, or scope surface is documented.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: accesstoken\n  type: apiKey\n  in: header\n  parameter: accesstoken\n  issuance: Tracxn platform > Data Solutions > API & Developer Tools > API Token\n  environments:\n  - production: https://platform.tracxn.com/api/2.2\n  - playground: https://platform.tracxn.com/api/2.2/playground\nunauthenticated_response:\n  status: 403\n  body:\n    errorCode: 403000000\n    message: Invalid web session access. No user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracxn/refs/heads/main/authentication/tracxn-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cloud Saas
- Market Intelligence
- Private Markets
- Venture Capital
- Startups
- Company Data
- Investors
- Funding
---
