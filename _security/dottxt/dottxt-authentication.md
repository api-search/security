---
api_key_in:
- header
api_specs:
- filename: dottxt-platform-openapi.yml
  format: yaml
  label: dottxt Platform API
  slug: dottxt-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dottxt/refs/heads/main/openapi/dottxt-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dottxt Authentication
name_suffix: Authentication
oauth_flows: []
overview: dottxt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dottxt
provider_slug: dottxt
scheme_count: 1
schemes:
- description: 'API key passed as a bearer token in the Authorization header: `Authorization: Bearer $DOTTXT_API_KEY`. Keys use the prefix `sk-dottxt-`. There is no OAuth flow; a single API key authenticates all requests.'
  header: Authorization
  key_prefix: sk-dottxt-
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dottxt-platform-openapi.yml
  type: http
slug: dottxt-authentication
source_filename: dottxt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/dottxt-platform-openapi.yml\ndocs: https://docs.dottxt.ai/api/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key passed as a bearer token in the Authorization header:\n    `Authorization: Bearer $DOTTXT_API_KEY`. Keys use the prefix `sk-dottxt-`.\n    There is no OAuth flow; a single API key authenticates all requests.\n  key_prefix: sk-dottxt-\n  header: Authorization\n  sources:\n  - openapi/dottxt-platform-openapi.yml\nnotes: >-\n  API access is currently gated by a waitlist form\n  (https://h1xbpbfsf0w.typeform.com/to/fwQNWmS8); keys are issued out of band,\n  not via a self-serve dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dottxt/refs/heads/main/authentication/dottxt-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Structured Outputs
- JSON Schema
- Machine Learning
- Developer Tools
- Constrained Decoding
---
