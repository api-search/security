---
api_key_in: []
api_specs:
- filename: kubernetes-services-endpointslices-api-openapi.yml
  format: yaml
  label: Kubernetes Services EndpointSlices API
  slug: kubernetes-services-endpointslices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-endpointslices-api-openapi.yml
- filename: kubernetes-services-gateway-api-openapi.yml
  format: yaml
  label: Kubernetes Services Gateway API
  slug: kubernetes-services-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-gateway-api-openapi.yml
- filename: kubernetes-services-gatewayclass-api-openapi.yml
  format: yaml
  label: Kubernetes Services GatewayClass API
  slug: kubernetes-services-gatewayclass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-gatewayclass-api-openapi.yml
- filename: kubernetes-services-grpcroute-api-openapi.yml
  format: yaml
  label: Kubernetes Services GRPCRoute API
  slug: kubernetes-services-grpcroute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-grpcroute-api-openapi.yml
- filename: kubernetes-services-httproute-api-openapi.yml
  format: yaml
  label: Kubernetes Services HTTPRoute API
  slug: kubernetes-services-httproute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-httproute-api-openapi.yml
- filename: kubernetes-services-ingress-api-openapi.yml
  format: yaml
  label: Kubernetes Services Ingress API
  slug: kubernetes-services-ingress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingress-api-openapi.yml
- filename: kubernetes-services-ingressclass-api-openapi.yml
  format: yaml
  label: Kubernetes Services IngressClass API
  slug: kubernetes-services-ingressclass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingressclass-api-openapi.yml
- filename: kubernetes-services-ingressstatus-api-openapi.yml
  format: yaml
  label: Kubernetes Services IngressStatus API
  slug: kubernetes-services-ingressstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingressstatus-api-openapi.yml
- filename: kubernetes-services-namespaces-api-openapi.yml
  format: yaml
  label: Kubernetes Services Namespaces API
  slug: kubernetes-services-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-namespaces-api-openapi.yml
- filename: kubernetes-services-networkpolicy-api-openapi.yml
  format: yaml
  label: Kubernetes Services NetworkPolicy API
  slug: kubernetes-services-networkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-networkpolicy-api-openapi.yml
- filename: kubernetes-services-services-api-openapi.yml
  format: yaml
  label: Kubernetes Services Services API
  slug: kubernetes-services-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-services-api-openapi.yml
- filename: kubernetes-services-servicestatus-api-openapi.yml
  format: yaml
  label: Kubernetes Services ServiceStatus API
  slug: kubernetes-services-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-servicestatus-api-openapi.yml
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
