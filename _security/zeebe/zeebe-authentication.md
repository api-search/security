---
api_key_in: []
api_specs:
- filename: zeebe-cluster-api-openapi.yml
  format: yaml
  label: Zeebe Cluster API
  slug: zeebe-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-cluster-api-openapi.yml
- filename: zeebe-deployments-api-openapi.yml
  format: yaml
  label: Zeebe Deployments API
  slug: zeebe-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-deployments-api-openapi.yml
- filename: zeebe-incidents-api-openapi.yml
  format: yaml
  label: Zeebe Incidents API
  slug: zeebe-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-incidents-api-openapi.yml
- filename: zeebe-jobs-api-openapi.yml
  format: yaml
  label: Zeebe Jobs API
  slug: zeebe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-jobs-api-openapi.yml
- filename: zeebe-messages-api-openapi.yml
  format: yaml
  label: Zeebe Messages API
  slug: zeebe-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-messages-api-openapi.yml
- filename: zeebe-process-instances-api-openapi.yml
  format: yaml
  label: Zeebe Process Instances API
  slug: zeebe-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-process-instances-api-openapi.yml
- filename: zeebe-resources-api-openapi.yml
  format: yaml
  label: Zeebe Resources API
  slug: zeebe-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-resources-api-openapi.yml
- filename: zeebe-signals-api-openapi.yml
  format: yaml
  label: Zeebe Signals API
  slug: zeebe-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-signals-api-openapi.yml
- filename: zeebe-user-tasks-api-openapi.yml
  format: yaml
  label: Zeebe User Tasks API
  slug: zeebe-user-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/openapi/zeebe-user-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zeebe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeebe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zeebe
provider_slug: zeebe
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zeebe-api.yml
  type: http
slug: zeebe-authentication
source_filename: zeebe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeebe-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zeebe-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeebe/refs/heads/main/authentication/zeebe-authentication.yml
summary_line: http · 1 scheme
tags:
- BPMN
- Camunda
- Cloud-Native
- Distributed Systems
- Java
- Microservices
- Process Automation
- Workflow Orchestration
---
