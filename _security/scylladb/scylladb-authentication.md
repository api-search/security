---
api_key_in: []
api_specs:
- filename: api-docs.json
  format: json
  label: ScyllaDB Cloud Management API
  slug: cloud-management-api
  spec_type: OpenAPI
  url: https://api.cloud.scylladb.com/api-docs.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scylladb Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScyllaDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScyllaDB
provider_slug: scylladb
scheme_count: 1
schemes:
- description: 'Authorization header, required in all authenticated requests.


    Header format: **Authorization: Bearer <token>**'
  name: Authorization
  scheme: bearer
  sources:
  - openapi/scylladb-cloud-management-api-openapi.yml
  type: http
slug: scylladb-authentication
source_filename: scylladb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scylladb-cloud-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  description: |-\n    Authorization header, required in all authenticated requests.\n\n    Header format: **Authorization: Bearer <token>**\n  sources:\n  - openapi/scylladb-cloud-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/authentication/scylladb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- NoSQL
- Cassandra Compatible
- DynamoDB Compatible
- Distributed Database
- Real-Time
- Vector Search
- Cloud Database
---
