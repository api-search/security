---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Black Duck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Black Duck secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Black Duck
provider_slug: black-duck
scheme_count: 2
schemes:
- description: 'A per-user API token generated in the Black Duck UI (My Access Tokens). Clients exchange the API token for a short-lived bearer token by POSTing to /api/tokens/authenticate with header "Authorization: token <api-token>", then use the returned bearerToken on subsequent requests.'
  in: header
  name: api-token
  type: apiKey
- description: 'Short-lived bearer token returned by /api/tokens/authenticate, sent as "Authorization: Bearer <token>".'
  name: bearer
  scheme: bearer
  type: http
slug: black-duck-authentication
source_filename: black-duck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://community.blackduck.com/s/article/Black-Duck-HUB-How-to-view-the-API-documentation\ndocs: https://documentation.blackduck.com/category/api\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  token_exchange: true\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  description: 'A per-user API token generated in the Black Duck UI (My Access Tokens). Clients\n    exchange the API token for a short-lived bearer token by POSTing to /api/tokens/authenticate\n    with header \"Authorization: token <api-token>\", then use the returned bearerToken on subsequent\n    requests.'\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Short-lived bearer token returned by /api/tokens/authenticate, sent as \"Authorization: Bearer <token>\".'\nnotes:\n- Black Duck OpenAPI and Postman artifacts are published per-server at /api-doc/openapi3-public.json\n  and /api-doc/postman-collection-public.json (require\
  \ an authenticated session on that server).\n- Coverity Connect and Polaris use their own authentication surfaces; this profile documents the\n  Black Duck SCA (Hub) REST API token flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/authentication/black-duck-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Enterprise
- Application Security
- Software Composition Analysis
- SAST
- DAST
- Open Source Security
- DevSecOps
- Vulnerability Management
---
