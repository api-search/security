---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numina secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Numina
provider_slug: cty
scheme_count: 1
schemes:
- bearer_format: JWT
  description: JWT bearer token presented in the Authorization header on every GraphQL request. Obtained through the API's authentication mutation. Access is granted per API user; developers request access at https://numina.co/api/.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.numina.co/
  type: http
slug: cty-authentication
source_filename: cty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.numina.co/\ndocs: https://developer.numina.co/\nnotes: >-\n  The Numina Graph API (\"Numina-Graph\") is a GraphQL API that authenticates\n  requests with JSON Web Tokens (JWT). A client obtains a token via an\n  authentication mutation, then presents it on subsequent GraphQL queries and\n  mutations using the HTTP Authorization header (Bearer <token>). No OpenAPI /\n  GraphQL SDL was captured for this repo, so schemes are documented from the\n  provider's public developer docs and API announcement rather than derived.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    JWT bearer token presented in the Authorization header on every GraphQL\n    request. Obtained through the API's authentication mutation. Access is\n    granted per API\
  \ user; developers request access at https://numina.co/api/.\n  sources:\n  - https://developer.numina.co/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cty/refs/heads/main/authentication/cty-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mobility
- Urban Planning
- Smart Cities
- Computer Vision
- Transportation
- GraphQL
- Sensors
- Street Intelligence
---
