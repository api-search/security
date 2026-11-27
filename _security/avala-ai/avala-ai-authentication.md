---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avala-ai-agents-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Agents API
  slug: avala-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-agents-api-openapi.yml
- filename: avala-ai-exports-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Exports API
  slug: avala-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-exports-api-openapi.yml
- filename: avala-ai-fleet-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Fleet API
  slug: avala-ai-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-fleet-api-openapi.yml
- filename: avala-ai-inference-providers-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Inference Providers API
  slug: avala-ai-inference-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-inference-providers-api-openapi.yml
- filename: avala-ai-models-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Models API
  slug: avala-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-models-api-openapi.yml
- filename: avala-ai-organizations-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Organizations API
  slug: avala-ai-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-organizations-api-openapi.yml
- filename: avala-ai-projects-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Projects API
  slug: avala-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-projects-api-openapi.yml
- filename: avala-ai-session-definitions-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Session Definitions API
  slug: avala-ai-session-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-session-definitions-api-openapi.yml
- filename: avala-ai-slices-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Slices API
  slug: avala-ai-slices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-slices-api-openapi.yml
- filename: avala-ai-storage-configs-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Storage Configs API
  slug: avala-ai-storage-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-storage-configs-api-openapi.yml
- filename: avala-ai-tasks-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Tasks API
  slug: avala-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-tasks-api-openapi.yml
- filename: avala-ai-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Webhook Deliveries API
  slug: avala-ai-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-webhook-deliveries-api-openapi.yml
- filename: avala-ai-webhooks-api-openapi.yml
  format: yaml
  label: Avala AI, Inc. Webhooks API
  slug: avala-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avala-ai/openapi/avala-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Avala AI, Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avala AI, Inc. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Avala AI, Inc.
provider_slug: avala-ai
scheme_count: 2
schemes:
- description: API key for authentication. Generate one in Mission Control Settings > Security & Identity.
  header: X-Avala-Api-Key
  in: header
  name: API_Key
  type: apiKey
- description: JWT token with 'JWT' prefix, e.g., 'JWT eyJhbGciOiJIUzI1NiIsInR...'
  header: Authorization
  in: header
  name: JWT
  type: apiKey
slug: avala-ai-authentication
source_filename: avala-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://avala.ai/docs/api-reference/openapi.json\nschemes:\n  - name: API_Key\n    type: apiKey\n    in: header\n    description: API key for authentication. Generate one in Mission Control Settings > Security & Identity.\n    header: X-Avala-Api-Key\n  - name: JWT\n    type: apiKey\n    in: header\n    description: JWT token with 'JWT' prefix, e.g., 'JWT eyJhbGciOiJIUzI1NiIsInR...'\n    header: Authorization\n"
source_yaml_url: https://artifacts.apis.io/avala-ai/authentication/avala-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Fleet Management
- Data
- Platform
- Machine Learning
---
