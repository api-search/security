---
api_key_in:
- header
api_specs:
- filename: tonic-ai-generate-data-api-openapi.yml
  format: yaml
  label: Tonic.ai Generate Data API
  slug: tonic-ai-generate-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/openapi/tonic-ai-generate-data-api-openapi.yml
- filename: tonic-ai-table-relationships-api-openapi.yml
  format: yaml
  label: Tonic.ai Table Relationships API
  slug: tonic-ai-table-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/openapi/tonic-ai-table-relationships-api-openapi.yml
- filename: tonic-ai-workspaces-api-openapi.yml
  format: yaml
  label: Tonic.ai Workspaces API
  slug: tonic-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/openapi/tonic-ai-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tonic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tonic.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tonic.ai
provider_slug: tonic-ai
scheme_count: 1
schemes:
- description: 'Tonic API key. Send as `Authorization: Apikey <token>`.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tonic-ai-openapi.yml
  type: apiKey
slug: tonic-ai-authentication
source_filename: tonic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tonic-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Tonic API key. Send as `Authorization: Apikey <token>`.'\n  sources:\n  - openapi/tonic-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/authentication/tonic-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Synthetic Data
- De-Identification
- Privacy
- Unstructured Data
- RAG Evaluation
- REST
- SDK
- Developer Tools
---
