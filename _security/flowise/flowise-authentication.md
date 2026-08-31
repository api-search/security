---
api_key_in: []
api_specs:
- filename: flowise-assistants-api-openapi.yml
  format: yaml
  label: Flowise assistants API
  slug: flowise-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-assistants-api-openapi.yml
- filename: flowise-attachments-api-openapi.yml
  format: yaml
  label: Flowise attachments API
  slug: flowise-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-attachments-api-openapi.yml
- filename: flowise-chatflows-api-openapi.yml
  format: yaml
  label: Flowise chatflows API
  slug: flowise-chatflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-chatflows-api-openapi.yml
- filename: flowise-chatmessage-api-openapi.yml
  format: yaml
  label: Flowise chatmessage API
  slug: flowise-chatmessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-chatmessage-api-openapi.yml
- filename: flowise-document-store-api-openapi.yml
  format: yaml
  label: Flowise document-store API
  slug: flowise-document-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-document-store-api-openapi.yml
- filename: flowise-feedback-api-openapi.yml
  format: yaml
  label: Flowise feedback API
  slug: flowise-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-feedback-api-openapi.yml
- filename: flowise-leads-api-openapi.yml
  format: yaml
  label: Flowise leads API
  slug: flowise-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-leads-api-openapi.yml
- filename: flowise-ping-api-openapi.yml
  format: yaml
  label: Flowise ping API
  slug: flowise-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-ping-api-openapi.yml
- filename: flowise-prediction-api-openapi.yml
  format: yaml
  label: Flowise prediction API
  slug: flowise-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-prediction-api-openapi.yml
- filename: flowise-tools-api-openapi.yml
  format: yaml
  label: Flowise tools API
  slug: flowise-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-tools-api-openapi.yml
- filename: flowise-upsert-history-api-openapi.yml
  format: yaml
  label: Flowise upsert-history API
  slug: flowise-upsert-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-upsert-history-api-openapi.yml
- filename: flowise-variables-api-openapi.yml
  format: yaml
  label: Flowise variables API
  slug: flowise-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-variables-api-openapi.yml
- filename: flowise-vector-api-openapi.yml
  format: yaml
  label: Flowise vector API
  slug: flowise-vector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-vector-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flowise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flowise
provider_slug: flowise
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flowise-openapi.yml
  type: http
slug: flowise-authentication
source_filename: flowise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flowise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/flowise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/authentication/flowise-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Agent Workflows
- Artificial Intelligence
- Large Language Models
- Low Code
- Visual Builder
- LangChain
- RAG
- Retrieval Augmented Generation
- Chatbots
- Open-Source
- Node.js
- TypeScript
---
