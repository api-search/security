---
api_key_in: []
api_specs:
- filename: etcd-auth-api-openapi.yml
  format: yaml
  label: Etcd Auth API
  slug: etcd-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-auth-api-openapi.yml
- filename: etcd-cluster-api-openapi.yml
  format: yaml
  label: Etcd Cluster API
  slug: etcd-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-cluster-api-openapi.yml
- filename: etcd-kv-api-openapi.yml
  format: yaml
  label: Etcd KV API
  slug: etcd-kv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-kv-api-openapi.yml
- filename: etcd-lease-api-openapi.yml
  format: yaml
  label: Etcd Lease API
  slug: etcd-lease-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-lease-api-openapi.yml
- filename: etcd-maintenance-api-openapi.yml
  format: yaml
  label: Etcd Maintenance API
  slug: etcd-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-maintenance-api-openapi.yml
- filename: etcd-watch-api-openapi.yml
  format: yaml
  label: Etcd Watch API
  slug: etcd-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-watch-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Etcd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Etcd secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Etcd
provider_slug: etcd
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the /auth/authenticate endpoint. Include in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/etcd-http-gateway-openapi.yml
  type: http
slug: etcd-authentication
source_filename: etcd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/etcd-http-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the /auth/authenticate endpoint. Include in the Authorization\n    header as \"Bearer {token}\".\n  sources:\n  - openapi/etcd-http-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/authentication/etcd-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud-Native
- Consensus
- Distributed Systems
- Graduated
- Key-Value Store
- Kubernetes
---
