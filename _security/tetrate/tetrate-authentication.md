---
api_key_in:
- header
api_specs:
- filename: tetrate-apis-api-openapi.yml
  format: yaml
  label: Tetrate APIs API
  slug: tetrate-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-apis-api-openapi.yml
- filename: tetrate-applications-api-openapi.yml
  format: yaml
  label: Tetrate Applications API
  slug: tetrate-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-applications-api-openapi.yml
- filename: tetrate-clusters-api-openapi.yml
  format: yaml
  label: Tetrate Clusters API
  slug: tetrate-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-clusters-api-openapi.yml
- filename: tetrate-gateway-groups-api-openapi.yml
  format: yaml
  label: Tetrate Gateway Groups API
  slug: tetrate-gateway-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-gateway-groups-api-openapi.yml
- filename: tetrate-organizations-api-openapi.yml
  format: yaml
  label: Tetrate Organizations API
  slug: tetrate-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-organizations-api-openapi.yml
- filename: tetrate-rbac-api-openapi.yml
  format: yaml
  label: Tetrate RBAC API
  slug: tetrate-rbac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-rbac-api-openapi.yml
- filename: tetrate-security-groups-api-openapi.yml
  format: yaml
  label: Tetrate Security Groups API
  slug: tetrate-security-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-security-groups-api-openapi.yml
- filename: tetrate-tenants-api-openapi.yml
  format: yaml
  label: Tetrate Tenants API
  slug: tetrate-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-tenants-api-openapi.yml
- filename: tetrate-traffic-groups-api-openapi.yml
  format: yaml
  label: Tetrate Traffic Groups API
  slug: tetrate-traffic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-traffic-groups-api-openapi.yml
- filename: tetrate-workspaces-api-openapi.yml
  format: yaml
  label: Tetrate Workspaces API
  slug: tetrate-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-workspaces-api-openapi.yml
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
