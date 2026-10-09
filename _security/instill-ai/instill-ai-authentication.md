---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: instill-ai-artifact-api-openapi.yml
  format: yaml
  label: Instill AI Artifact API
  slug: instill-ai-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-artifact-api-openapi.yml
- filename: instill-ai-connection-api-openapi.yml
  format: yaml
  label: Instill AI Connection API
  slug: instill-ai-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-connection-api-openapi.yml
- filename: instill-ai-integration-api-openapi.yml
  format: yaml
  label: Instill AI Integration API
  slug: instill-ai-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-integration-api-openapi.yml
- filename: instill-ai-metrics-api-openapi.yml
  format: yaml
  label: Instill AI Metrics API
  slug: instill-ai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-metrics-api-openapi.yml
- filename: instill-ai-model-api-openapi.yml
  format: yaml
  label: Instill AI Model API
  slug: instill-ai-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-model-api-openapi.yml
- filename: instill-ai-namespace-api-openapi.yml
  format: yaml
  label: Instill AI Namespace API
  slug: instill-ai-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-namespace-api-openapi.yml
- filename: instill-ai-pipeline-api-openapi.yml
  format: yaml
  label: Instill AI Pipeline API
  slug: instill-ai-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/openapi/instill-ai-pipeline-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Instill Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instill AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instill AI
provider_slug: instill-ai
scheme_count: 1
schemes:
- description: Enter the token with the `Bearer ` prefix, e.g. `Bearer instill_sk_***`
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/instill-ai-openapi.yml
  type: apiKey
slug: instill-ai-authentication
source_filename: instill-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/instill-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Enter the token with the `Bearer ` prefix, e.g. `Bearer instill_sk_***`\n  sources:\n  - openapi/instill-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instill-ai/refs/heads/main/authentication/instill-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Unstructured Data
- Data Pipelines
- RAG
- Open Source
- LLM
---
