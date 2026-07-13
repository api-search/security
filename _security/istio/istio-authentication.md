---
api_key_in: []
api_specs:
- filename: istio-networking-api-openapi.yml
  format: yaml
  label: Istio Networking API
  slug: networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-networking-api-openapi.yml
- filename: istio-security-api-openapi.yml
  format: yaml
  label: Istio Security API
  slug: security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-security-api-openapi.yml
- filename: istio-telemetry-api-openapi.yml
  format: yaml
  label: Istio Telemetry API
  slug: telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-telemetry-api-openapi.yml
- filename: istio-extensions-api-openapi.yml
  format: yaml
  label: Istio Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-extensions-api-openapi.yml
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
