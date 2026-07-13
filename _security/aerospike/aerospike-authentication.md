---
api_key_in: []
api_specs:
- filename: aerospike-openapi.yml
  format: yaml
  label: Aerospike REST Gateway
  slug: rest-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospike/refs/heads/main/openapi/aerospike-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aerospike Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aerospike secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aerospike
provider_slug: aerospike
scheme_count: 1
schemes:
- description: HTTP Basic credentials are forwarded by the REST Gateway to the Aerospike security subsystem when enabled. When Aerospike security is disabled the gateway accepts requests without authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/aerospike-openapi.yml
  type: http
slug: aerospike-authentication
source_filename: aerospike-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aerospike-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic credentials are forwarded by the REST Gateway to the Aerospike security\n    subsystem when enabled. When Aerospike security is disabled the gateway accepts requests\n    without authentication.\n  sources:\n  - openapi/aerospike-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerospike/refs/heads/main/authentication/aerospike-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- NoSQL
- Real-Time
- Key-Value
- In-Memory
- Vector Database
- High Performance
---
