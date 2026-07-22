---
api_key_in: []
api_specs:
- filename: rigetti-computing-qcs-openapi-original.yml
  format: yaml
  label: Rigetti QCS API
  slug: rigetti-qcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rigetti-computing/refs/heads/main/openapi/rigetti-computing-qcs-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rigetti Computing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rigetti Computing secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rigetti Computing
provider_slug: rigetti-computing
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A JSON web token with `sub` or `uid` claim, as well as `groups` claim. If the token is absent, invalid or expired, the client will receive a 401 response. If the token is valid, the server uses the claims to authorize the request, which may result in a 403 response.
  name: JWTBearer
  scheme: bearer
  sources:
  - openapi/rigetti-computing-qcs-openapi-original.yml
  type: http
slug: rigetti-computing-authentication
source_filename: rigetti-computing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rigetti-computing-qcs-openapi-original.yml\ndocs: https://qcs.rigetti.com/auth/token\nmodel:\n  protocol: oauth2\n  identity_provider: Okta\n  token_format: JWT\n  token_lifetime: 24h\n  authorize: \"Download an access token from https://qcs.rigetti.com/auth/token; use the access_token value (not the whole JSON) as Authorization: Bearer <jwt>.\"\n  request_access: https://www.rigetti.com/get-quantum\n  legacy_note: \"The same account/token works against the legacy Forest API at https://forest-server.qcs.rigetti.com.\"\nsummary:\n  types:\n  - http\nschemes:\n- name: JWTBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A JSON web token with `sub` or `uid` claim, as well as `groups` claim. If the\n    token is absent, invalid or expired, the client will receive a 401 response. If the token\n    is valid, the server uses the claims to authorize the request, which may result in a 403\n    response.\n\
  \  sources:\n  - openapi/rigetti-computing-qcs-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rigetti-computing/refs/heads/main/authentication/rigetti-computing-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Quantum Computing
- Quantum Cloud
- Developer Tools
- SDKs
- Superconducting Qubits
- Scientific Computing
- Deep Tech
---
