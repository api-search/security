---
api_key_in: []
api_specs:
- filename: turbonomic-actions-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Actions API
  slug: turbonomic-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-actions-api-openapi.yml
- filename: turbonomic-authentication-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Authentication API
  slug: turbonomic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-authentication-api-openapi.yml
- filename: turbonomic-entities-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Entities API
  slug: turbonomic-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-entities-api-openapi.yml
- filename: turbonomic-groups-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Groups API
  slug: turbonomic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-groups-api-openapi.yml
- filename: turbonomic-markets-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Markets API
  slug: turbonomic-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-markets-api-openapi.yml
- filename: turbonomic-policies-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Policies API
  slug: turbonomic-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-policies-api-openapi.yml
- filename: turbonomic-statistics-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Statistics API
  slug: turbonomic-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-statistics-api-openapi.yml
- filename: turbonomic-targets-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Targets API
  slug: turbonomic-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-targets-api-openapi.yml
- filename: turbonomic-templates-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Templates API
  slug: turbonomic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-templates-api-openapi.yml
- filename: turbonomic-topology-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Topology API
  slug: turbonomic-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-topology-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turbonomic Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM Turbonomic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBM Turbonomic
provider_slug: turbonomic
scheme_count: 1
schemes:
- description: Bearer token obtained by calling POST /api/v3/login with username and password. Include in the Authorization header as 'Bearer {token}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/turbonomic-rest-api-openapi.yml
  type: http
slug: turbonomic-authentication
source_filename: turbonomic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turbonomic-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained by calling POST /api/v3/login with username and password.\n    Include in the Authorization header as 'Bearer {token}'.\n  sources:\n  - openapi/turbonomic-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/authentication/turbonomic-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Resource Management
- Cloud Cost Optimization
- Cloud Management
- Hybrid Cloud
- IBM
- Kubernetes
- Multi-Cloud
- Workload Optimization
---
