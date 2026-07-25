---
api_key_in:
- header
api_specs:
- filename: nomad-acl-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad ACL API
  slug: nomad-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-acl-api-openapi.yml
- filename: nomad-agent-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Agent API
  slug: nomad-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-agent-api-openapi.yml
- filename: nomad-allocations-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Allocations API
  slug: nomad-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-allocations-api-openapi.yml
- filename: nomad-deployments-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Deployments API
  slug: nomad-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-deployments-api-openapi.yml
- filename: nomad-evaluations-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Evaluations API
  slug: nomad-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-evaluations-api-openapi.yml
- filename: nomad-jobs-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Jobs API
  slug: nomad-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-jobs-api-openapi.yml
- filename: nomad-namespaces-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Namespaces API
  slug: nomad-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-namespaces-api-openapi.yml
- filename: nomad-node-pools-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Node Pools API
  slug: nomad-node-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-node-pools-api-openapi.yml
- filename: nomad-nodes-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Nodes API
  slug: nomad-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-nodes-api-openapi.yml
- filename: nomad-operator-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Operator API
  slug: nomad-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-operator-api-openapi.yml
- filename: nomad-regions-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Regions API
  slug: nomad-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-regions-api-openapi.yml
- filename: nomad-scaling-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Scaling API
  slug: nomad-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-scaling-api-openapi.yml
- filename: nomad-search-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Search API
  slug: nomad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-search-api-openapi.yml
- filename: nomad-service-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Service API
  slug: nomad-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-service-api-openapi.yml
- filename: nomad-services-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Services API
  slug: nomad-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-services-api-openapi.yml
- filename: nomad-status-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Status API
  slug: nomad-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-status-api-openapi.yml
- filename: nomad-system-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad System API
  slug: nomad-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-system-api-openapi.yml
- filename: nomad-variables-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Variables API
  slug: nomad-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-variables-api-openapi.yml
- filename: nomad-volumes-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Volumes API
  slug: nomad-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-volumes-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nomad Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Nomad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HashiCorp Nomad
provider_slug: nomad
scheme_count: 2
schemes:
- description: ACL token passed via the X-Nomad-Token request header.
  in: header
  name: nomadToken
  parameter: X-Nomad-Token
  sources:
  - openapi/nomad-http-api-openapi.yml
  type: apiKey
- description: ACL token passed via the Authorization header with Bearer scheme.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nomad-http-api-openapi.yml
  type: http
slug: nomad-authentication
source_filename: nomad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nomad-http-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: nomadToken\n  type: apiKey\n  in: header\n  parameter: X-Nomad-Token\n  description: ACL token passed via the X-Nomad-Token request header.\n  sources:\n  - openapi/nomad-http-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: ACL token passed via the Authorization header with Bearer scheme.\n  sources:\n  - openapi/nomad-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/authentication/nomad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Workload Orchestration
- Container Orchestration
- Scheduling
- Infrastructure
- DevOps
---
