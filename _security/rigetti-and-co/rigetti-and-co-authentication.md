---
api_key_in: []
api_specs:
- filename: rigetti-and-co-qcs-openapi.yml
  format: yaml
  label: Rigetti QCS API
  slug: rigetti-qcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rigetti-and-co/refs/heads/main/openapi/rigetti-and-co-qcs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rigetti And Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rigetti & Co secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rigetti & Co
provider_slug: rigetti-and-co
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A JSON web token with `sub` or `uid` claim, as well as `groups` claim. If the token is absent, invalid or expired, the client will receive a 401 response. If the token is valid, the server uses the claims to authorize the request, which may result in a 403 response.
  name: JWTBearer
  scheme: bearer
  sources:
  - openapi/rigetti-and-co-qcs-openapi.yml
  type: http
slug: rigetti-and-co-authentication
source_filename: rigetti-and-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rigetti-and-co-qcs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWTBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A JSON web token with `sub` or `uid` claim, as well as `groups` claim. If the\n    token is absent, invalid or expired, the client will receive a 401 response. If the token\n    is valid, the server uses the claims to authorize the request, which may result in a 403\n    response.\n  sources:\n  - openapi/rigetti-and-co-qcs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rigetti-and-co/refs/heads/main/authentication/rigetti-and-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Quantum Computing
- Quantum
- Infrastructure
- Developers
- Cloud Computing
- QPU
- API
---
