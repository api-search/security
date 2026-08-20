---
api_key_in: []
api_specs:
- filename: trigger-dev-batches-api-openapi.yml
  format: yaml
  label: Trigger.dev Batches API
  slug: trigger-dev-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-batches-api-openapi.yml
- filename: trigger-dev-deployments-api-openapi.yml
  format: yaml
  label: Trigger.dev Deployments API
  slug: trigger-dev-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-deployments-api-openapi.yml
- filename: trigger-dev-environment-variables-api-openapi.yml
  format: yaml
  label: Trigger.dev Environment Variables API
  slug: trigger-dev-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-environment-variables-api-openapi.yml
- filename: trigger-dev-query-api-openapi.yml
  format: yaml
  label: Trigger.dev Query API
  slug: trigger-dev-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-query-api-openapi.yml
- filename: trigger-dev-queues-api-openapi.yml
  format: yaml
  label: Trigger.dev Queues API
  slug: trigger-dev-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-queues-api-openapi.yml
- filename: trigger-dev-runs-api-openapi.yml
  format: yaml
  label: Trigger.dev Runs API
  slug: trigger-dev-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-runs-api-openapi.yml
- filename: trigger-dev-schedules-api-openapi.yml
  format: yaml
  label: Trigger.dev Schedules API
  slug: trigger-dev-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-schedules-api-openapi.yml
- filename: trigger-dev-tasks-api-openapi.yml
  format: yaml
  label: Trigger.dev Tasks API
  slug: trigger-dev-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-tasks-api-openapi.yml
- filename: trigger-dev-waitpoints-api-openapi.yml
  format: yaml
  label: Trigger.dev Waitpoints API
  slug: trigger-dev-waitpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-waitpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trigger Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trigger.dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trigger.dev
provider_slug: trigger-dev
scheme_count: 1
schemes:
- description: Secret API key (starts with tr_dev_, tr_prod_, or tr_stg_). Set TRIGGER_SECRET_KEY environment variable or pass in Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trigger-dev-management-openapi.yml
  type: http
slug: trigger-dev-authentication
source_filename: trigger-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trigger-dev-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Secret API key (starts with tr_dev_, tr_prod_, or tr_stg_). Set TRIGGER_SECRET_KEY\n    environment variable or pass in Authorization header.\n  sources:\n  - openapi/trigger-dev-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/authentication/trigger-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer-First
- Workflow-Automation
- Background Jobs
- Durable Execution
- TypeScript
- AI Agents
- Real-Time
- Open-Source
---
