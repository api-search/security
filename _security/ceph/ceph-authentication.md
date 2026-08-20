---
api_key_in: []
api_specs:
- filename: ceph-auth-api-openapi.yml
  format: yaml
  label: Ceph Auth API
  slug: ceph-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-auth-api-openapi.yml
- filename: ceph-cluster-api-openapi.yml
  format: yaml
  label: Ceph Cluster API
  slug: ceph-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-cluster-api-openapi.yml
- filename: ceph-configuration-api-openapi.yml
  format: yaml
  label: Ceph Configuration API
  slug: ceph-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-configuration-api-openapi.yml
- filename: ceph-crush-api-openapi.yml
  format: yaml
  label: Ceph CRUSH API
  slug: ceph-crush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-crush-api-openapi.yml
- filename: ceph-daemon-api-openapi.yml
  format: yaml
  label: Ceph Daemon API
  slug: ceph-daemon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-daemon-api-openapi.yml
- filename: ceph-user-api-openapi.yml
  format: yaml
  label: Ceph User API
  slug: ceph-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/openapi/ceph-user-api-openapi.yml
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
- Open-Source
- Software-Defined Storage
---
