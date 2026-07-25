---
api_key_in:
- header
api_specs:
- filename: circleci-runner-api-openapi.yml
  format: yaml
  label: CircleCI Self-Hosted Runner API
  slug: runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-runner-api-openapi.yml
- filename: circleci-webhooks-asyncapi.yml
  format: yaml
  label: CircleCI Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/asyncapi/circleci-webhooks-asyncapi.yml
- filename: circleci-artifact-api-openapi.yml
  format: yaml
  label: CircleCI Artifact API
  slug: circleci-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-artifact-api-openapi.yml
- filename: circleci-build-api-openapi.yml
  format: yaml
  label: CircleCI Build API
  slug: circleci-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-build-api-openapi.yml
- filename: circleci-context-api-openapi.yml
  format: yaml
  label: CircleCI Context API
  slug: circleci-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-context-api-openapi.yml
- filename: circleci-insights-api-openapi.yml
  format: yaml
  label: CircleCI Insights API
  slug: circleci-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-insights-api-openapi.yml
- filename: circleci-job-api-openapi.yml
  format: yaml
  label: CircleCI Job API
  slug: circleci-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-job-api-openapi.yml
- filename: circleci-pipeline-api-openapi.yml
  format: yaml
  label: CircleCI Pipeline API
  slug: circleci-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-pipeline-api-openapi.yml
- filename: circleci-project-api-openapi.yml
  format: yaml
  label: CircleCI Project API
  slug: circleci-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-project-api-openapi.yml
- filename: circleci-resource-class-api-openapi.yml
  format: yaml
  label: CircleCI Resource Class API
  slug: circleci-resource-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-resource-class-api-openapi.yml
- filename: circleci-runner-task-api-openapi.yml
  format: yaml
  label: CircleCI Runner Task API
  slug: circleci-runner-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-runner-task-api-openapi.yml
- filename: circleci-schedule-api-openapi.yml
  format: yaml
  label: CircleCI Schedule API
  slug: circleci-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-schedule-api-openapi.yml
- filename: circleci-ssh-key-api-openapi.yml
  format: yaml
  label: CircleCI SSH Key API
  slug: circleci-ssh-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-ssh-key-api-openapi.yml
- filename: circleci-test-metadata-api-openapi.yml
  format: yaml
  label: CircleCI Test Metadata API
  slug: circleci-test-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-test-metadata-api-openapi.yml
- filename: circleci-user-api-openapi.yml
  format: yaml
  label: CircleCI User API
  slug: circleci-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-user-api-openapi.yml
- filename: circleci-webhook-api-openapi.yml
  format: yaml
  label: CircleCI Webhook API
  slug: circleci-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-webhook-api-openapi.yml
- filename: circleci-workflow-api-openapi.yml
  format: yaml
  label: CircleCI Workflow API
  slug: circleci-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-workflow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circleci Authentication
name_suffix: Authentication
oauth_flows: []
overview: CircleCI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CircleCI
provider_slug: circleci
scheme_count: 3
schemes:
- description: Personal API token for authenticating with the CircleCI API. Can also be passed as a query parameter.
  in: header
  name: apiToken
  parameter: Circle-Token
  sources:
  - openapi/circleci-rest-api-v1-openapi.yml
  - openapi/circleci-rest-api-v2-openapi.yml
  - openapi/circleci-runner-api-openapi.yml
  type: apiKey
- description: HTTP basic authentication using a personal API token as the username with an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/circleci-rest-api-v2-openapi.yml
  type: http
- description: Resource class token generated when creating a new resource class. This token is only displayed once and cannot be retrieved again.
  name: resourceClassToken
  scheme: bearer
  sources:
  - openapi/circleci-runner-api-openapi.yml
  type: http
slug: circleci-authentication
source_filename: circleci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circleci-rest-api-v1-openapi.yml, openapi/circleci-rest-api-v2-openapi.yml,\n  openapi/circleci-runner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Circle-Token\n  description: Personal API token for authenticating with the CircleCI API. Can also be passed\n    as a query parameter.\n  sources:\n  - openapi/circleci-rest-api-v1-openapi.yml\n  - openapi/circleci-rest-api-v2-openapi.yml\n  - openapi/circleci-runner-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP basic authentication using a personal API token as the username with an\n    empty password.\n  sources:\n  - openapi/circleci-rest-api-v2-openapi.yml\n- name: resourceClassToken\n  type: http\n  scheme: bearer\n  description: Resource class token generated when creating a new resource class. This token\n    is only\
  \ displayed once and cannot be retrieved again.\n  sources:\n  - openapi/circleci-runner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/authentication/circleci-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
---
