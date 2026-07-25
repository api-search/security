---
api_key_in:
- header
api_specs:
- filename: hashicorp-nomad-acl-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad ACL API
  slug: hashicorp-nomad-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-acl-api-openapi.yml
- filename: hashicorp-nomad-allocations-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Allocations API
  slug: hashicorp-nomad-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-allocations-api-openapi.yml
- filename: hashicorp-nomad-deployments-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Deployments API
  slug: hashicorp-nomad-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-deployments-api-openapi.yml
- filename: hashicorp-nomad-evaluations-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Evaluations API
  slug: hashicorp-nomad-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-evaluations-api-openapi.yml
- filename: hashicorp-nomad-jobs-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Jobs API
  slug: hashicorp-nomad-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-jobs-api-openapi.yml
- filename: hashicorp-nomad-namespaces-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Namespaces API
  slug: hashicorp-nomad-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-namespaces-api-openapi.yml
- filename: hashicorp-nomad-nodes-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad Nodes API
  slug: hashicorp-nomad-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-nodes-api-openapi.yml
- filename: hashicorp-nomad-system-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad System API
  slug: hashicorp-nomad-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hashicorp Nomad Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Nomad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HashiCorp Nomad
provider_slug: hashicorp-nomad
scheme_count: 2
schemes:
- in: header
  name: NomadToken
  parameter: X-Nomad-Token
  sources:
  - openapi/hashicorp-nomad-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hashicorp-nomad-openapi.yml
  type: http
slug: hashicorp-nomad-authentication
source_filename: hashicorp-nomad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hashicorp-nomad-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: NomadToken\n  type: apiKey\n  in: header\n  parameter: X-Nomad-Token\n  sources:\n  - openapi/hashicorp-nomad-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hashicorp-nomad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/authentication/hashicorp-nomad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Containers
- HashiCorp
- Multi-Cloud
- Orchestration
- Scheduling
- Workloads
---
