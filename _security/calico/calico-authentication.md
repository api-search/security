---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Calico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calico secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calico
provider_slug: calico
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Kubernetes service account bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/calico-openapi.yml
  type: http
slug: calico-authentication
source_filename: calico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/calico-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account bearer token.\n  sources:\n  - openapi/calico-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/authentication/calico-authentication.yml
summary_line: http · 1 scheme
tags:
- CNI
- Containers
- eBPF
- Kubernetes
- Network Policy
- Network Security
- Networking
- Open Source
- Service Mesh
---
