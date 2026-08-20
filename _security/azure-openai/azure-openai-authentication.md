---
api_key_in:
- header
api_specs:
- filename: azure-openai-asyncapi.yml
  format: yaml
  label: Azure OpenAI Inference REST API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/asyncapi/azure-openai-asyncapi.yml
- filename: azure-openai-audio-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Audio API
  slug: azure-openai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/openapi/azure-openai-audio-api-openapi.yml
- filename: azure-openai-chat-completions-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Chat Completions API
  slug: azure-openai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/openapi/azure-openai-chat-completions-api-openapi.yml
- filename: azure-openai-completions-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Completions API
  slug: azure-openai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/openapi/azure-openai-completions-api-openapi.yml
- filename: azure-openai-embeddings-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Embeddings API
  slug: azure-openai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/openapi/azure-openai-embeddings-api-openapi.yml
- filename: azure-openai-images-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Images API
  slug: azure-openai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/openapi/azure-openai-images-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Openai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azure OpenAI Service secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azure OpenAI Service
provider_slug: azure-openai
scheme_count: 2
schemes:
- description: Azure OpenAI resource API key
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/azure-openai-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-openai-openapi.yml
  type: oauth2
slug: azure-openai-authentication
source_filename: azure-openai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-openai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Azure OpenAI resource API key\n  sources:\n  - openapi/azure-openai-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n  sources:\n  - openapi/azure-openai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/authentication/azure-openai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- LLM
- Generative AI
- Azure
- OpenAI
- Foundation Models
- Chat Completions
- Embeddings
---
