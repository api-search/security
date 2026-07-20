---
api_key_in:
- header
api_specs:
- filename: fluence-openapi-original.yml
  format: yaml
  label: Fluence API
  slug: fluence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fluence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluence secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fluence
provider_slug: fluence
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token issued by Fluence
  name: access_jwt_token
  scheme: bearer
  sources:
  - openapi/fluence-openapi-original.yml
  type: http
- in: header
  name: api_key
  parameter: X-API-KEY
  sources:
  - openapi/fluence-openapi-original.yml
  type: apiKey
slug: fluence-authentication
source_filename: fluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fluence-openapi-original.yml\ndocs: https://fluence.dev/docs/build/api/overview\nnotes: >-\n  Primary auth is an API key sent in the X-API-KEY header (create/manage at\n  console.fluence.network/settings/api-keys); a missing or invalid key returns forbidden.\n  A JWT bearer token (access_jwt_token) is used for console/session flows. API keys carry\n  permission scopes — see scopes/fluence-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: access_jwt_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token issued by Fluence\n  sources:\n  - openapi/fluence-openapi-original.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/fluence-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/authentication/fluence-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto Web3
- Cloud Compute
- DePIN
- GPU
- Infrastructure
- Virtual Machines
- AI Infrastructure
- Decentralized Cloud
---
