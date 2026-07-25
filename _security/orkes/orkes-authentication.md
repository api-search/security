---
api_key_in: []
api_specs:
- filename: orkes-authentication-api-openapi.yml
  format: yaml
  label: Orkes Authentication API
  slug: orkes-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-authentication-api-openapi.yml
- filename: orkes-human-tasks-api-openapi.yml
  format: yaml
  label: Orkes Human Tasks API
  slug: orkes-human-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-human-tasks-api-openapi.yml
- filename: orkes-schedules-api-openapi.yml
  format: yaml
  label: Orkes Schedules API
  slug: orkes-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-schedules-api-openapi.yml
- filename: orkes-secrets-api-openapi.yml
  format: yaml
  label: Orkes Secrets API
  slug: orkes-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-secrets-api-openapi.yml
- filename: orkes-task-metadata-api-openapi.yml
  format: yaml
  label: Orkes Task Metadata API
  slug: orkes-task-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-task-metadata-api-openapi.yml
- filename: orkes-tasks-api-openapi.yml
  format: yaml
  label: Orkes Tasks API
  slug: orkes-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-tasks-api-openapi.yml
- filename: orkes-workflow-execution-api-openapi.yml
  format: yaml
  label: Orkes Workflow Execution API
  slug: orkes-workflow-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-workflow-execution-api-openapi.yml
- filename: orkes-workflow-metadata-api-openapi.yml
  format: yaml
  label: Orkes Workflow Metadata API
  slug: orkes-workflow-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-workflow-metadata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orkes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orkes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orkes
provider_slug: orkes
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/orkes-conductor-api.yml
  type: http
slug: orkes-authentication
source_filename: orkes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orkes-conductor-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/orkes-conductor-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/authentication/orkes-authentication.yml
summary_line: http · 1 scheme
tags:
- Microservices
---
