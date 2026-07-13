---
api_key_in: []
api_specs:
- filename: kgateway-kubernetes-gateway-api-openapi.yml
  format: yaml
  label: Kgateway Kubernetes Gateway API
  slug: kgateway-kubernetes-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/openapi/kgateway-kubernetes-gateway-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kgateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kgateway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kgateway
provider_slug: kgateway
scheme_count: 1
schemes:
- description: Kubernetes API bearer token authentication. Use a service account token or kubeconfig token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kgateway-kubernetes-gateway-api-openapi.yml
  type: http
slug: kgateway-authentication
source_filename: kgateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kgateway-kubernetes-gateway-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Kubernetes API bearer token authentication. Use a service account token or kubeconfig\n    token.\n  sources:\n  - openapi/kgateway-kubernetes-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/authentication/kgateway-authentication.yml
summary_line: http · 1 scheme
tags:
- Gateways
---
