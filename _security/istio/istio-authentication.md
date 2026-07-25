---
api_key_in: []
api_specs:
- filename: istio-telemetry-api-openapi.yml
  format: yaml
  label: Istio Telemetry API
  slug: telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-telemetry-api-openapi.yml
- filename: istio-authorizationpolicy-api-openapi.yml
  format: yaml
  label: Istio AuthorizationPolicy API
  slug: istio-authorizationpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-authorizationpolicy-api-openapi.yml
- filename: istio-destinationrule-api-openapi.yml
  format: yaml
  label: Istio DestinationRule API
  slug: istio-destinationrule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-destinationrule-api-openapi.yml
- filename: istio-gateway-api-openapi.yml
  format: yaml
  label: Istio Gateway API
  slug: istio-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-gateway-api-openapi.yml
- filename: istio-peerauthentication-api-openapi.yml
  format: yaml
  label: Istio PeerAuthentication API
  slug: istio-peerauthentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-peerauthentication-api-openapi.yml
- filename: istio-requestauthentication-api-openapi.yml
  format: yaml
  label: Istio RequestAuthentication API
  slug: istio-requestauthentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-requestauthentication-api-openapi.yml
- filename: istio-serviceentry-api-openapi.yml
  format: yaml
  label: Istio ServiceEntry API
  slug: istio-serviceentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-serviceentry-api-openapi.yml
- filename: istio-sidecar-api-openapi.yml
  format: yaml
  label: Istio Sidecar API
  slug: istio-sidecar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-sidecar-api-openapi.yml
- filename: istio-virtualservice-api-openapi.yml
  format: yaml
  label: Istio VirtualService API
  slug: istio-virtualservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-virtualservice-api-openapi.yml
- filename: istio-wasmplugin-api-openapi.yml
  format: yaml
  label: Istio WasmPlugin API
  slug: istio-wasmplugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-wasmplugin-api-openapi.yml
- filename: istio-workloadentry-api-openapi.yml
  format: yaml
  label: Istio WorkloadEntry API
  slug: istio-workloadentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-workloadentry-api-openapi.yml
- filename: istio-workloadgroup-api-openapi.yml
  format: yaml
  label: Istio WorkloadGroup API
  slug: istio-workloadgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-workloadgroup-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Istio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Istio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Istio
provider_slug: istio
scheme_count: 1
schemes:
- description: Kubernetes API server bearer token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/istio-extensions-api-openapi.yml
  - openapi/istio-networking-api-openapi.yml
  - openapi/istio-security-api-openapi.yml
  - openapi/istio-telemetry-api-openapi.yml
  type: http
slug: istio-authentication
source_filename: istio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/istio-extensions-api-openapi.yml, openapi/istio-networking-api-openapi.yml,\n  openapi/istio-security-api-openapi.yml, openapi/istio-telemetry-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Kubernetes API server bearer token authentication\n  sources:\n  - openapi/istio-extensions-api-openapi.yml\n  - openapi/istio-networking-api-openapi.yml\n  - openapi/istio-security-api-openapi.yml\n  - openapi/istio-telemetry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/authentication/istio-authentication.yml
summary_line: http · 1 scheme
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
---
