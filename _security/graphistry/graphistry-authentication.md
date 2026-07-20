---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Graphistry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphistry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphistry
provider_slug: graphistry
scheme_count: 1
schemes:
- bearer_format: JWT
  description: JWT obtained by POSTing username/password to api-token-auth/, then sent as an Authorization bearer token on subsequent REST calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  token_endpoints:
    obtain: POST /api-token-auth/   {"username":"...","password":"..."}
    refresh: POST /api-token-refresh/   {"token":"..."}
    verify: POST /api-token-verify/   {"token":"..."}
  token_lifetime: ~1 hour; refreshable within 24 hours, then full re-authentication required
  type: http
slug: graphistry-authentication
source_filename: graphistry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://hub.graphistry.com/docs/api/1/rest/auth/\ndocs: https://hub.graphistry.com/docs/api/1/rest/auth/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\n  notes: Graphistry Hub REST API uses short-lived JWT bearer tokens (api=3). Legacy\n    api=1/2 authentication paths were removed in PyGraphistry 0.56.0.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: JWT obtained by POSTing username/password to api-token-auth/, then sent\n    as an Authorization bearer token on subsequent REST calls.\n  token_endpoints:\n    obtain: POST /api-token-auth/   {\"username\":\"...\",\"password\":\"...\"}\n    refresh: POST /api-token-refresh/   {\"token\":\"...\"}\n    verify: POST /api-token-verify/   {\"token\":\"...\"}\n  token_lifetime: ~1 hour; refreshable within 24 hours, then full re-authentication\n    required\n  sources:\
  \ [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphistry/refs/heads/main/authentication/graphistry-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Graph Analytics
- Graph Visualization
- GPU
- Network Analysis
- Data Visualization
- Graph Query
- Machine Learning
- Cybersecurity
---
