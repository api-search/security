---
anonymous_access: false
api_key_in: []
api_specs:
- filename: empiriolabs-ai-chatcompletions-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Chat Completions API
  slug: empiriolabs-ai-chatcompletions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-chatcompletions-api-openapi.yml
- filename: empiriolabs-ai-completions-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Completions API
  slug: empiriolabs-ai-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-completions-api-openapi.yml
- filename: empiriolabs-ai-gemini-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Gemini API
  slug: empiriolabs-ai-gemini-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-gemini-api-openapi.yml
- filename: empiriolabs-ai-messages-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Messages API
  slug: empiriolabs-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-messages-api-openapi.yml
- filename: empiriolabs-ai-models-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Models API
  slug: empiriolabs-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-models-api-openapi.yml
- filename: empiriolabs-ai-responses-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Responses API
  slug: empiriolabs-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-responses-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Empiriolabs Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmpirioLabs AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EmpirioLabs AI
provider_slug: empiriolabs-ai
scheme_count: 2
schemes:
- description: Bearer token with sk-empiriolabs- prefix
  in: header
  name: Authorization
  type: apiKey
- authorizationUrl: https://platform.empiriolabs.ai/auth/login
  flow: authorizationCode
  scopes: {}
  tokenUrl: https://platform.empiriolabs.ai/auth/token
  type: oauth2
slug: empiriolabs-ai-authentication
source_filename: empiriolabs-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.empiriolabs.ai/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token with sk-empiriolabs- prefix\"\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://platform.empiriolabs.ai/auth/login\n    tokenUrl: https://platform.empiriolabs.ai/auth/token\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/empiriolabs-ai/authentication/empiriolabs-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Inference
- Cloud
- Platform
---
