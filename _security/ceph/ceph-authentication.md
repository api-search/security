---
api_key_in: []
api_specs:
- filename: api.json
  format: json
  label: Ceph RESTful API
  slug: restful-api
  spec_type: OpenAPI
  url: https://{manager_host}:{dashboard_port}/docs/api.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ceph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ceph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ceph
provider_slug: ceph
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT obtained from POST /api/auth.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ceph-openapi.yml
  type: http
slug: ceph-authentication
source_filename: ceph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ceph-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT obtained from POST /api/auth.\n  sources:\n  - openapi/ceph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/authentication/ceph-authentication.yml
summary_line: http · 1 scheme
tags:
- Storage
- Distributed Storage
- Object Storage
- Block Storage
- File Storage
- Open Source
- Software-Defined Storage
---
