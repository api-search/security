---
api_key_in:
- query
api_specs:
- filename: kvdb-openapi.yml
  format: yaml
  label: KVdb
  slug: kvdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kvdb/refs/heads/main/openapi/kvdb-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kvdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: KVdb secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KVdb
provider_slug: kvdb
scheme_count: 2
schemes:
- description: Bucket secret key passed via HTTP Basic auth
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kvdb-openapi.yml
  type: http
- in: query
  name: secretKeyQuery
  parameter: secret_key
  sources:
  - openapi/kvdb-openapi.yml
  type: apiKey
slug: kvdb-authentication
source_filename: kvdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kvdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Bucket secret key passed via HTTP Basic auth\n  sources:\n  - openapi/kvdb-openapi.yml\n- name: secretKeyQuery\n  type: apiKey\n  in: query\n  parameter: secret_key\n  sources:\n  - openapi/kvdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kvdb/refs/heads/main/authentication/kvdb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Databases
- Key-Value
- NoSQL
- Serverless
---
