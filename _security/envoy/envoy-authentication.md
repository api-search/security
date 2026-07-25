---
api_key_in: []
api_specs:
- filename: envoy-certificates-api-openapi.yml
  format: yaml
  label: Envoy Certificates API
  slug: envoy-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-certificates-api-openapi.yml
- filename: envoy-chat-api-openapi.yml
  format: yaml
  label: Envoy Chat API
  slug: envoy-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-chat-api-openapi.yml
- filename: envoy-clusters-api-openapi.yml
  format: yaml
  label: Envoy Clusters API
  slug: envoy-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-clusters-api-openapi.yml
- filename: envoy-configuration-api-openapi.yml
  format: yaml
  label: Envoy Configuration API
  slug: envoy-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-configuration-api-openapi.yml
- filename: envoy-health-api-openapi.yml
  format: yaml
  label: Envoy Health API
  slug: envoy-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-health-api-openapi.yml
- filename: envoy-listeners-api-openapi.yml
  format: yaml
  label: Envoy Listeners API
  slug: envoy-listeners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-listeners-api-openapi.yml
- filename: envoy-logging-api-openapi.yml
  format: yaml
  label: Envoy Logging API
  slug: envoy-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-logging-api-openapi.yml
- filename: envoy-models-api-openapi.yml
  format: yaml
  label: Envoy Models API
  slug: envoy-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-models-api-openapi.yml
- filename: envoy-runtime-api-openapi.yml
  format: yaml
  label: Envoy Runtime API
  slug: envoy-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-runtime-api-openapi.yml
- filename: envoy-server-api-openapi.yml
  format: yaml
  label: Envoy Server API
  slug: envoy-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-server-api-openapi.yml
- filename: envoy-statistics-api-openapi.yml
  format: yaml
  label: Envoy Statistics API
  slug: envoy-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-statistics-api-openapi.yml
- filename: envoy-text-completions-api-openapi.yml
  format: yaml
  label: Envoy Text Completions API
  slug: envoy-text-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-text-completions-api-openapi.yml
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
