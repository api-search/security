---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inferenceindexer-ai-auth-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Auth API
  slug: inferenceindexer-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-auth-api-openapi.yml
- filename: inferenceindexer-ai-embeddings-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Embeddings API
  slug: inferenceindexer-ai-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-embeddings-api-openapi.yml
- filename: inferenceindexer-ai-explain-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Explain API
  slug: inferenceindexer-ai-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-explain-api-openapi.yml
- filename: inferenceindexer-ai-export-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Export API
  slug: inferenceindexer-ai-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-export-api-openapi.yml
- filename: inferenceindexer-ai-health-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Health API
  slug: inferenceindexer-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-health-api-openapi.yml
- filename: inferenceindexer-ai-inferenceindexer-api-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai InferenceIndexer API
  slug: inferenceindexer-ai-inferenceindexer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-inferenceindexer-api-api-openapi.yml
- filename: inferenceindexer-ai-models-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Models API
  slug: inferenceindexer-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-models-api-openapi.yml
- filename: inferenceindexer-ai-providers-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Providers API
  slug: inferenceindexer-ai-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-providers-api-openapi.yml
- filename: inferenceindexer-ai-recommend-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Recommend API
  slug: inferenceindexer-ai-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-recommend-api-openapi.yml
- filename: inferenceindexer-ai-sit-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Sit API
  slug: inferenceindexer-ai-sit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-sit-api-openapi.yml
- filename: inferenceindexer-ai-tpi-api-openapi.yml
  format: yaml
  label: InferenceIndexer.ai Tpi API
  slug: inferenceindexer-ai-tpi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferenceindexer-ai/openapi/inferenceindexer-ai-tpi-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InferenceIndexer.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: InferenceIndexer.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: InferenceIndexer.ai
provider_slug: inferenceindexer-ai
scheme_count: 2
schemes:
- evidence: curl -X POST https://api.inferenceindexer.ai/v1/auth/anonymous Returns a key instantly, valid on the free tier (10,000 requests/day, 30 days of history).
  header: Authorization
  how_to_obtain: POST https://api.inferenceindexer.ai/v1/auth/anonymous returns a key instantly
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'Pass your API key in the Authorization header: Authorization : Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Sign up with an email and retrieve the API key from the dashboard
  location: header
  name: Bearer
  type: http-bearer
slug: inferenceindexer-ai-authentication
source_filename: inferenceindexer-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.inferenceindexer.ai/for-agents
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.inferenceindexer.ai/for-agents\nsources:\n- https://www.inferenceindexer.ai/for-agents\n- https://www.inferenceindexer.ai/api-docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: curl -X POST https://api.inferenceindexer.ai/v1/auth/anonymous Returns a key instantly, valid on the free tier (10,000 requests/day,\n    30 days of history).\n  location: header\n  header: Authorization\n  how_to_obtain: POST https://api.inferenceindexer.ai/v1/auth/anonymous returns a key instantly\n- type: http-bearer\n  name: Bearer\n  evidence: 'Pass your API key in the Authorization header: Authorization : Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up with an email and retrieve the API key from the dashboard\ndocs: https://www.inferenceindexer.ai/for-agents\n"
source_yaml_url: https://artifacts.apis.io/inferenceindexer-ai/authentication/inferenceindexer-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Inference
- Pricing
- Data
- Platform
- Company
---
