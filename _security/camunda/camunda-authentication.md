---
api_key_in: []
api_specs:
- filename: camunda-cluster-api-openapi.yml
  format: yaml
  label: Camunda Cluster API
  slug: camunda-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-cluster-api-openapi.yml
- filename: camunda-decisions-api-openapi.yml
  format: yaml
  label: Camunda Decisions API
  slug: camunda-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-decisions-api-openapi.yml
- filename: camunda-deployments-api-openapi.yml
  format: yaml
  label: Camunda Deployments API
  slug: camunda-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-deployments-api-openapi.yml
- filename: camunda-incidents-api-openapi.yml
  format: yaml
  label: Camunda Incidents API
  slug: camunda-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-incidents-api-openapi.yml
- filename: camunda-jobs-api-openapi.yml
  format: yaml
  label: Camunda Jobs API
  slug: camunda-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-jobs-api-openapi.yml
- filename: camunda-messages-api-openapi.yml
  format: yaml
  label: Camunda Messages API
  slug: camunda-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-messages-api-openapi.yml
- filename: camunda-process-definitions-api-openapi.yml
  format: yaml
  label: Camunda Process Definitions API
  slug: camunda-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-process-definitions-api-openapi.yml
- filename: camunda-process-instances-api-openapi.yml
  format: yaml
  label: Camunda Process Instances API
  slug: camunda-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-process-instances-api-openapi.yml
- filename: camunda-signals-api-openapi.yml
  format: yaml
  label: Camunda Signals API
  slug: camunda-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-signals-api-openapi.yml
- filename: camunda-user-tasks-api-openapi.yml
  format: yaml
  label: Camunda User Tasks API
  slug: camunda-user-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-user-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Camunda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Camunda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Camunda
provider_slug: camunda
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/camunda-8-api.yml
  type: http
slug: camunda-authentication
source_filename: camunda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camunda-8-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/camunda-8-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/authentication/camunda-authentication.yml
summary_line: http · 1 scheme
tags:
- BPMN
- Business Process Management
- Process Automation
- Workflow
---
