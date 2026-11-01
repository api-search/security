---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bithuman-ai-account-api-openapi.yml
  format: yaml
  label: bithuman-ai Account API
  slug: bithuman-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-account-api-openapi.yml
- filename: bithuman-ai-agent-context-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Context API
  slug: bithuman-ai-agent-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-context-api-openapi.yml
- filename: bithuman-ai-agent-generation-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Generation API
  slug: bithuman-ai-agent-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-generation-api-openapi.yml
- filename: bithuman-ai-agent-management-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Management API
  slug: bithuman-ai-agent-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-management-api-openapi.yml
- filename: bithuman-ai-api-secrets-api-openapi.yml
  format: yaml
  label: bithuman-ai API secrets API
  slug: bithuman-ai-api-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-api-secrets-api-openapi.yml
- filename: bithuman-ai-authentication-api-openapi.yml
  format: yaml
  label: bithuman-ai Authentication API
  slug: bithuman-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-authentication-api-openapi.yml
- filename: bithuman-ai-billing-api-openapi.yml
  format: yaml
  label: bithuman-ai Billing API
  slug: bithuman-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-billing-api-openapi.yml
- filename: bithuman-ai-dynamics-api-openapi.yml
  format: yaml
  label: bithuman-ai Dynamics API
  slug: bithuman-ai-dynamics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-dynamics-api-openapi.yml
- filename: bithuman-ai-embedding-api-openapi.yml
  format: yaml
  label: bithuman-ai Embedding API
  slug: bithuman-ai-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-embedding-api-openapi.yml
- filename: bithuman-ai-files-api-openapi.yml
  format: yaml
  label: bithuman-ai Files API
  slug: bithuman-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-files-api-openapi.yml
- filename: bithuman-ai-knowledge-api-openapi.yml
  format: yaml
  label: bithuman-ai Knowledge API
  slug: bithuman-ai-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-knowledge-api-openapi.yml
- filename: bithuman-ai-providers-api-openapi.yml
  format: yaml
  label: bithuman-ai Providers API
  slug: bithuman-ai-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-providers-api-openapi.yml
- filename: bithuman-ai-realtime-api-openapi.yml
  format: yaml
  label: bithuman-ai Realtime API
  slug: bithuman-ai-realtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-realtime-api-openapi.yml
- filename: bithuman-ai-runtime-sessions-api-openapi.yml
  format: yaml
  label: bithuman-ai Runtime sessions API
  slug: bithuman-ai-runtime-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-runtime-sessions-api-openapi.yml
- filename: bithuman-ai-self-hosting-api-openapi.yml
  format: yaml
  label: bithuman-ai Self Hosting API
  slug: bithuman-ai-self-hosting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-self-hosting-api-openapi.yml
- filename: bithuman-ai-status-api-openapi.yml
  format: yaml
  label: bithuman-ai Status API
  slug: bithuman-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-status-api-openapi.yml
- filename: bithuman-ai-video-api-openapi.yml
  format: yaml
  label: bithuman-ai Video API
  slug: bithuman-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-video-api-openapi.yml
- filename: bithuman-ai-webhooks-api-openapi.yml
  format: yaml
  label: bithuman-ai Webhooks API
  slug: bithuman-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bithuman Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: bithuman-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: bithuman-ai
provider_slug: bithuman-ai
scheme_count: 2
schemes:
- description: Your bitHuman API secret. Get one at https://www.bithuman.ai/developer/api-keys
  in: header
  name: api-secret
  type: apiKey
- description: 'The same API secret, sent as Authorization: Bearer <api-secret>. Self-hosted runtimes send it this way.'
  scheme: bearer
  type: http
slug: bithuman-ai-authentication
source_filename: bithuman-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://docs.bithuman.ai/api/openapi.yaml\nschemes:\n  - type: apiKey\n    name: api-secret\n    in: header\n    description: \"Your bitHuman API secret. Get one at https://www.bithuman.ai/developer/api-keys\"\n  - type: http\n    scheme: bearer\n    description: \"The same API secret, sent as Authorization: Bearer <api-secret>. Self-hosted runtimes send it this way.\"\n"
source_yaml_url: https://artifacts.apis.io/bithuman-ai/authentication/bithuman-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Avatar
- Real-time
- Platform
---
