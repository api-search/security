---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nimble Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nimble Storage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nimble Storage
provider_slug: nimble-storage
scheme_count: 1
schemes:
- description: Session token returned by POST https://<array>:5392/v1/tokens with a JSON body containing the array username and password. The returned session_token is sent as the X-Auth-Token request header on all subsequent calls. Tokens expire after an idle timeout and are revoked by DELETE on the token object.
  in: header
  name: session-token
  parameter_name: X-Auth-Token
  sources:
  - docs
  token_endpoint: https://<array>:5392/v1/tokens
  type: apiKey
slug: nimble-storage-authentication
source_filename: nimble-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://infosight.hpe.com/InfoSight/media/cms/active/public/pubs_REST_API_Reference_NOS_51x.whz/\ndocs: https://developer.hpe.com/platform/hpe-nimble-storage/home/\nnotes: >-\n  The NimbleOS REST API uses session-token authentication. A client first POSTs\n  array credentials (username/password) to the tokens endpoint to obtain a\n  session_token, then presents that token in the X-Auth-Token header on every\n  subsequent request. Authentication and the API are served per-array (on-prem\n  appliance), not from a central hosted endpoint.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: session-token\n    type: apiKey\n    in: header\n    parameter_name: X-Auth-Token\n    description: >-\n      Session token returned by POST https://<array>:5392/v1/tokens with a JSON\n      body containing the array username and password. The returned\n      session_token is sent as the X-Auth-Token\
  \ request header on all subsequent\n      calls. Tokens expire after an idle timeout and are revoked by DELETE on the\n      token object.\n    token_endpoint: https://<array>:5392/v1/tokens\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble-storage/refs/heads/main/authentication/nimble-storage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Big Data
- Storage
- Data Storage
- Infrastructure
- Enterprise
- HPE
---
