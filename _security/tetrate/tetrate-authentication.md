---
api_key_in:
- header
api_specs:
- filename: tetrate-service-bridge-openapi.yml
  format: yaml
  label: Tetrate Service Bridge REST API
  slug: tsb-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-service-bridge-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tetrate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tetrate secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tetrate
provider_slug: tetrate
scheme_count: 2
schemes:
- description: HTTP Basic authentication with TSB username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/tetrate-service-bridge-openapi.yml
  type: http
- description: JWT token authentication using the x-tetrate-token header
  in: header
  name: JWTToken
  parameter: x-tetrate-token
  sources:
  - openapi/tetrate-service-bridge-openapi.yml
  type: apiKey
slug: tetrate-authentication
source_filename: tetrate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tetrate-service-bridge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with TSB username and password\n  sources:\n  - openapi/tetrate-service-bridge-openapi.yml\n- name: JWTToken\n  type: apiKey\n  in: header\n  parameter: x-tetrate-token\n  description: JWT token authentication using the x-tetrate-token header\n  sources:\n  - openapi/tetrate-service-bridge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/authentication/tetrate-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Enterprise
- Envoy
- Istio
- Kubernetes
- Service Mesh
---
