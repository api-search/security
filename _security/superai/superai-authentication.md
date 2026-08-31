---
api_key_in:
- header
api_specs:
- filename: superai-auth-api-openapi.yml
  format: yaml
  label: Super.ai auth API
  slug: superai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-auth-api-openapi.yml
- filename: superai-files-api-openapi.yml
  format: yaml
  label: Super.ai files API
  slug: superai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-files-api-openapi.yml
- filename: superai-flow-executions-api-openapi.yml
  format: yaml
  label: Super.ai flow-executions API
  slug: superai-flow-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-flow-executions-api-openapi.yml
- filename: superai-flows-api-openapi.yml
  format: yaml
  label: Super.ai flows API
  slug: superai-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-flows-api-openapi.yml
- filename: superai-human-review-tasks-api-openapi.yml
  format: yaml
  label: Super.ai human-review-tasks API
  slug: superai-human-review-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-human-review-tasks-api-openapi.yml
- filename: superai-integrations-api-openapi.yml
  format: yaml
  label: Super.ai integrations API
  slug: superai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-integrations-api-openapi.yml
- filename: superai-models-api-openapi.yml
  format: yaml
  label: Super.ai models API
  slug: superai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-models-api-openapi.yml
- filename: superai-organizations-api-openapi.yml
  format: yaml
  label: Super.ai organizations API
  slug: superai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-organizations-api-openapi.yml
- filename: superai-plugins-api-openapi.yml
  format: yaml
  label: Super.ai plugins API
  slug: superai-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-plugins-api-openapi.yml
- filename: superai-profile-api-openapi.yml
  format: yaml
  label: Super.ai profile API
  slug: superai-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-profile-api-openapi.yml
- filename: superai-service-accounts-api-openapi.yml
  format: yaml
  label: Super.ai service-accounts API
  slug: superai-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-service-accounts-api-openapi.yml
- filename: superai-sso-api-openapi.yml
  format: yaml
  label: Super.ai sso API
  slug: superai-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-sso-api-openapi.yml
- filename: superai-task-data-api-openapi.yml
  format: yaml
  label: Super.ai task-data API
  slug: superai-task-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-task-data-api-openapi.yml
- filename: superai-task-executions-api-openapi.yml
  format: yaml
  label: Super.ai task-executions API
  slug: superai-task-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-task-executions-api-openapi.yml
- filename: superai-task-executors-api-openapi.yml
  format: yaml
  label: Super.ai task-executors API
  slug: superai-task-executors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-task-executors-api-openapi.yml
- filename: superai-task-outputs-api-openapi.yml
  format: yaml
  label: Super.ai task-outputs API
  slug: superai-task-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-task-outputs-api-openapi.yml
- filename: superai-task-tags-api-openapi.yml
  format: yaml
  label: Super.ai task-tags API
  slug: superai-task-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-task-tags-api-openapi.yml
- filename: superai-webhook-data-api-openapi.yml
  format: yaml
  label: Super.ai webhook-data API
  slug: superai-webhook-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-webhook-data-api-openapi.yml
- filename: superai-worker-groups-api-openapi.yml
  format: yaml
  label: Super.ai worker-groups API
  slug: superai-worker-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-worker-groups-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Superai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Super.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Super.ai
provider_slug: superai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT Bearer token authentication. Include your access token in the Authorization header as: `Bearer YOUR_ACCESS_TOKEN`


    Example:

    ```

    Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...

    ```'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/superai-flows-openapi-original.json
  type: http
- description: 'API key authentication. Include your API key in the X-API-Key header as: `X-API-Key YOUR_API_KEY`


    Example:

    ```

    X-API-Key: saf_1234567890

    ```'
  in: header
  name: APIKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/superai-flows-openapi-original.json
  type: apiKey
slug: superai-authentication
source_filename: superai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/superai-flows-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT Bearer token authentication. Include your access token in the Authorization header as: `Bearer YOUR_ACCESS_TOKEN`\n\n    Example:\n    ```\n    Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...\n    ```\n  sources:\n  - openapi/superai-flows-openapi-original.json\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key authentication. Include your API key in the X-API-Key header as: `X-API-Key YOUR_API_KEY`\n\n    Example:\n    ```\n    X-API-Key: saf_1234567890\n    ```\n  sources:\n  - openapi/superai-flows-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/authentication/superai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai Enterprise Software
- Intelligent Document Processing
- Document Processing
- Workflow Orchestration
- Automation
- Human In The Loop
- Artificial Intelligence
- REST API
---
