---
api_key_in: []
api_specs:
- filename: riak-openapi.yml
  format: yaml
  label: Riak KV HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Riak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Riak KV secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Riak KV
provider_slug: riak
scheme_count: 1
schemes:
- description: 'Riak KV supports optional security with HTTPS and basic auth or

    certificate-based authentication. By default, the HTTP listener is

    unauthenticated.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/riak-openapi.yml
  type: http
slug: riak-authentication
source_filename: riak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/riak-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Riak KV supports optional security with HTTPS and basic auth or\n    certificate-based authentication. By default, the HTTP listener is\n    unauthenticated.\n  sources:\n  - openapi/riak-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/authentication/riak-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- NoSQL
- Key-Value Store
- Distributed Systems
- Open Source
- Basho
- CRDT
---
