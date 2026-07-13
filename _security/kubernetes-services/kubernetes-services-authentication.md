---
api_key_in: []
api_specs:
- filename: kubernetes-services-openapi.yml
  format: yaml
  label: Kubernetes Services
  slug: kubernetes-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-openapi.yml
- filename: kubernetes-ingress-openapi.yml
  format: yaml
  label: Kubernetes Ingress
  slug: kubernetes-ingress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-ingress-openapi.yml
- filename: kubernetes-gateway-api-openapi.yml
  format: yaml
  label: Kubernetes Gateway API
  slug: kubernetes-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-gateway-api-openapi.yml
- filename: kubernetes-endpoint-slices-openapi.yml
  format: yaml
  label: Kubernetes EndpointSlices
  slug: kubernetes-endpoint-slices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-endpoint-slices-openapi.yml
- filename: kubernetes-network-policies-openapi.yml
  format: yaml
  label: Kubernetes Network Policies
  slug: kubernetes-network-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-network-policies-openapi.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Kubernetes Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubernetes Services secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kubernetes Services
provider_slug: kubernetes-services
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Kubernetes service account or user bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kubernetes-endpoint-slices-openapi.yml
  - openapi/kubernetes-gateway-api-openapi.yml
  - openapi/kubernetes-ingress-openapi.yml
  - openapi/kubernetes-network-policies-openapi.yml
  - openapi/kubernetes-services-openapi.yml
  type: http
- description: Client TLS certificate signed by the cluster CA.
  name: clientCertificate
  sources:
  - openapi/kubernetes-endpoint-slices-openapi.yml
  - openapi/kubernetes-gateway-api-openapi.yml
  - openapi/kubernetes-ingress-openapi.yml
  - openapi/kubernetes-network-policies-openapi.yml
  - openapi/kubernetes-services-openapi.yml
  type: mutualTLS
slug: kubernetes-services-authentication
source_filename: kubernetes-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kubernetes-endpoint-slices-openapi.yml, openapi/kubernetes-gateway-api-openapi.yml,\n  openapi/kubernetes-ingress-openapi.yml, openapi/kubernetes-network-policies-openapi.yml, openapi/kubernetes-services-openapi.yml\nsummary:\n  types:\n  - http\n  - mutualTLS\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account or user bearer token.\n  sources:\n  - openapi/kubernetes-endpoint-slices-openapi.yml\n  - openapi/kubernetes-gateway-api-openapi.yml\n  - openapi/kubernetes-ingress-openapi.yml\n  - openapi/kubernetes-network-policies-openapi.yml\n  - openapi/kubernetes-services-openapi.yml\n- name: clientCertificate\n  type: mutualTLS\n  description: Client TLS certificate signed by the cluster CA.\n  sources:\n  - openapi/kubernetes-endpoint-slices-openapi.yml\n  - openapi/kubernetes-gateway-api-openapi.yml\n  - openapi/kubernetes-ingress-openapi.yml\n\
  \  - openapi/kubernetes-network-policies-openapi.yml\n  - openapi/kubernetes-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/authentication/kubernetes-services-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Container Orchestration
- Kubernetes
- Load Balancing
- Networking
- Service Discovery
---
