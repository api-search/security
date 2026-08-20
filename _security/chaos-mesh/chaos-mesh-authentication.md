---
api_key_in: []
api_specs:
- filename: chaos-mesh-archives-api-openapi.yml
  format: yaml
  label: Chaos Mesh Archives API
  slug: chaos-mesh-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-archives-api-openapi.yml
- filename: chaos-mesh-common-api-openapi.yml
  format: yaml
  label: Chaos Mesh Common API
  slug: chaos-mesh-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-common-api-openapi.yml
- filename: chaos-mesh-events-api-openapi.yml
  format: yaml
  label: Chaos Mesh Events API
  slug: chaos-mesh-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-events-api-openapi.yml
- filename: chaos-mesh-experiments-api-openapi.yml
  format: yaml
  label: Chaos Mesh Experiments API
  slug: chaos-mesh-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-experiments-api-openapi.yml
- filename: chaos-mesh-schedules-api-openapi.yml
  format: yaml
  label: Chaos Mesh Schedules API
  slug: chaos-mesh-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-schedules-api-openapi.yml
- filename: chaos-mesh-templates-api-openapi.yml
  format: yaml
  label: Chaos Mesh Templates API
  slug: chaos-mesh-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-templates-api-openapi.yml
- filename: chaos-mesh-workflows-api-openapi.yml
  format: yaml
  label: Chaos Mesh Workflows API
  slug: chaos-mesh-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chaos Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chaos Mesh secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chaos Mesh
provider_slug: chaos-mesh
scheme_count: 1
schemes:
- description: Bearer token for authenticating API requests. Typically a Kubernetes service account token with RBAC permissions to read/write Chaos Mesh custom resources in the target namespaces.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chaos-mesh-dashboard-openapi.yml
  type: http
slug: chaos-mesh-authentication
source_filename: chaos-mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chaos-mesh-dashboard-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for authenticating API requests. Typically a Kubernetes service\n    account token with RBAC permissions to read/write Chaos Mesh custom resources in the target\n    namespaces.\n  sources:\n  - openapi/chaos-mesh-dashboard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/authentication/chaos-mesh-authentication.yml
summary_line: http · 1 scheme
tags:
- Chaos Engineering
- Cloud-Native
- CNCF
- Fault Injection
- Kubernetes
- Observability
- Open-Source
- Reliability
- Resilience
- Testing
---
