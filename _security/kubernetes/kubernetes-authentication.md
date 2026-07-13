---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: Kubernetes API
  slug: kubernetes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubernetes/kubernetes/master/api/openapi-spec/swagger.json
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Kubernetes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubernetes secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kubernetes
provider_slug: kubernetes
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Kubernetes service account token or user token issued by the cluster's authentication provider. Include in the Authorization header as 'Bearer <token>'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kubernetes-api-openapi.yml
  type: http
- description: Client certificate authentication using a TLS certificate issued by the cluster's certificate authority.
  name: clientCertificate
  sources:
  - openapi/kubernetes-api-openapi.yml
  type: mutualTLS
slug: kubernetes-authentication
source_filename: kubernetes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kubernetes-api-openapi.yml\nsummary:\n  types:\n  - http\n  - mutualTLS\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account token or user token issued by the cluster's authentication\n    provider. Include in the Authorization header as 'Bearer <token>'.\n  sources:\n  - openapi/kubernetes-api-openapi.yml\n- name: clientCertificate\n  type: mutualTLS\n  description: Client certificate authentication using a TLS certificate issued by the cluster's\n    certificate authority.\n  sources:\n  - openapi/kubernetes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/authentication/kubernetes-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Automation
- Cloud Native
- CNCF
- Containers
- Deployment
- Open Source
- Orchestration
- Scaling
---
