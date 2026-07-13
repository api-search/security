---
api_key_in: []
api_specs:
- filename: crossplane-kubernetes-api-openapi.yml
  format: yaml
  label: Crossplane Kubernetes API
  slug: crossplane-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/openapi/crossplane-kubernetes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Crossplane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crossplane secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crossplane
provider_slug: crossplane
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Kubernetes service account token or user bearer token for authenticating with the Kubernetes API server. RBAC policies control which Crossplane resources each identity can access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/crossplane-kubernetes-api-openapi.yml
  type: http
slug: crossplane-authentication
source_filename: crossplane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crossplane-kubernetes-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account token or user bearer token for authenticating with\n    the Kubernetes API server. RBAC policies control which Crossplane resources each identity\n    can access.\n  sources:\n  - openapi/crossplane-kubernetes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/authentication/crossplane-authentication.yml
summary_line: http · 1 scheme
tags:
- Apache 2.0
- CNCF
- Cloud Native
- Composition
- Control Plane
- Custom Resource Definitions
- Graduated
- Infrastructure as Code
- Kubernetes
- Multi-Cloud
- Open Source
- Platform Engineering
- Providers
---
