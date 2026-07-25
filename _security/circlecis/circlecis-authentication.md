---
api_key_in:
- header
api_specs:
- filename: circlecis-context-api-openapi.yml
  format: yaml
  label: CircleCI Context API
  slug: circlecis-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-context-api-openapi.yml
- filename: circlecis-job-api-openapi.yml
  format: yaml
  label: CircleCI Job API
  slug: circlecis-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-job-api-openapi.yml
- filename: circlecis-pipeline-api-openapi.yml
  format: yaml
  label: CircleCI Pipeline API
  slug: circlecis-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-pipeline-api-openapi.yml
- filename: circlecis-project-api-openapi.yml
  format: yaml
  label: CircleCI Project API
  slug: circlecis-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-project-api-openapi.yml
- filename: circlecis-user-api-openapi.yml
  format: yaml
  label: CircleCI User API
  slug: circlecis-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-user-api-openapi.yml
- filename: circlecis-workflow-api-openapi.yml
  format: yaml
  label: CircleCI Workflow API
  slug: circlecis-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-workflow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circlecis Authentication
name_suffix: Authentication
oauth_flows: []
overview: CircleCI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CircleCI
provider_slug: circlecis
scheme_count: 2
schemes:
- description: CircleCI personal API token.
  in: header
  name: apiTokenAuth
  parameter: Circle-Token
  sources:
  - openapi/circlecis-openapi.yml
  type: apiKey
- description: HTTP Basic with API token as username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/circlecis-openapi.yml
  type: http
slug: circlecis-authentication
source_filename: circlecis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circlecis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Circle-Token\n  description: CircleCI personal API token.\n  sources:\n  - openapi/circlecis-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with API token as username.\n  sources:\n  - openapi/circlecis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/authentication/circlecis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CI/CD
- Continuous Deployment
- Continuous Integration
- DevOps
- Pipelines
- Workflows
---
