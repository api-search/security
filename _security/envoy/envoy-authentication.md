---
api_key_in: []
api_specs:
- filename: envoy-admin-api-openapi.yml
  format: yaml
  label: Envoy Admin API
  slug: envoy-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-admin-api-openapi.yml
- filename: envoy-ai-gateway-openapi.yml
  format: yaml
  label: Envoy AI Gateway API
  slug: envoy-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-ai-gateway-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Envoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Envoy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Envoy
provider_slug: envoy
scheme_count: 1
schemes:
- description: Bearer token authentication. The token is configured per route in the AIGatewayRoute Kubernetes custom resource. For AI provider backends, the gateway may automatically translate the bearer token to the appropriate provider-specific authentication mechanism.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/envoy-ai-gateway-openapi.yml
  type: http
slug: envoy-authentication
source_filename: envoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/envoy-ai-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. The token is configured per route in the AIGatewayRoute\n    Kubernetes custom resource. For AI provider backends, the gateway may automatically translate\n    the bearer token to the appropriate provider-specific authentication mechanism.\n  sources:\n  - openapi/envoy-ai-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/authentication/envoy-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- Load Balancing
- Proxy
- Service Mesh
---
