---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-openai-openapi.yml
  format: yaml
  label: Azure OpenAI Service API
  slug: azure-openai-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-openai/refs/heads/main/openapi/microsoft-azure-openai-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Openai Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure OpenAI Service secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure OpenAI Service
provider_slug: microsoft-azure-openai
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/microsoft-azure-openai-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-openai-openapi.yml
  type: oauth2
slug: microsoft-azure-openai-authentication
source_filename: microsoft-azure-openai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-openai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/microsoft-azure-openai-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/microsoft-azure-openai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-openai/refs/heads/main/authentication/microsoft-azure-openai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI
- Embeddings
- GPT
- Generative AI
- Large Language Models
- OpenAI
---
