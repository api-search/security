---
api_key_in: []
api_specs:
- filename: client-libraries
  format: yaml
  label: SpiceDB Permissions API
  slug: spicedb-permissions-api
  spec_type: OpenAPI
  url: https://authzed.com/docs/spicedb/getting-started/client-libraries
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Authzed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authzed secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Authzed
provider_slug: authzed
scheme_count: 1
schemes:
- description: 'SpiceDB preshared-key. Pass as Authorization: Bearer <preshared-key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/authzed-spicedb-permissions-api-openapi.yml
  type: http
slug: authzed-authentication
source_filename: authzed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authzed-spicedb-permissions-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'SpiceDB preshared-key. Pass as Authorization: Bearer <preshared-key>'\n  sources:\n  - openapi/authzed-spicedb-permissions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authzed/refs/heads/main/authentication/authzed-authentication.yml
summary_line: http · 1 scheme
tags:
- Authorization
- Access Control
- Permissions
- Zanzibar
- SpiceDB
- gRPC
- REST
- Relationship-Based Access Control
- ReBAC
- Fine-Grained Authorization
- Identity
- Security
---
