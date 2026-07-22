---
api_key_in:
- header
api_specs:
- filename: superai-flows-openapi-original.json
  format: json
  label: SuperAI Flows API
  slug: superai-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-flows-openapi-original.json
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
