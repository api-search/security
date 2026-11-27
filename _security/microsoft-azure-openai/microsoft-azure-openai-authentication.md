---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: azure-openai-asyncapi.yml
  format: yaml
  label: Azure OpenAI Inference REST API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/azure-openai/asyncapi/azure-openai-asyncapi.yml
- filename: microsoft-azure-openai-batch-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Batch: API'
  slug: microsoft-azure-openai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-batch-api-openapi.yml
- filename: microsoft-azure-openai-deployments-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Deployments API
  slug: microsoft-azure-openai-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-deployments-api-openapi.yml
- filename: microsoft-azure-openai-files-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Files: API'
  slug: microsoft-azure-openai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-files-api-openapi.yml
- filename: microsoft-azure-openai-fine-tuning-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Fine Tuning: API'
  slug: microsoft-azure-openai-fine-tuning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-fine-tuning-api-openapi.yml
- filename: microsoft-azure-openai-models-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Models: API'
  slug: microsoft-azure-openai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-models-api-openapi.yml
- filename: microsoft-azure-openai-uploadfile-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Upload File: API'
  slug: microsoft-azure-openai-uploadfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-uploadfile-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Azure OpenAI Service Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure OpenAI Service secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure OpenAI Service
provider_slug: microsoft-azure-openai
scheme_count: 2
schemes:
- description: Provide your Cognitive Services Azure OpenAI account key here.
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/microsoft-azure-openai-batch-api-openapi.yml
  - openapi/microsoft-azure-openai-deployments-api-openapi.yml
  - openapi/microsoft-azure-openai-files-api-openapi.yml
  - openapi/microsoft-azure-openai-fine-tuning-api-openapi.yml
  - openapi/microsoft-azure-openai-models-api-openapi.yml
  - openapi/microsoft-azure-openai-uploadfile-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: implicit
    scopes: 0
  name: bearer
  sources:
  - openapi/microsoft-azure-openai-deployments-api-openapi.yml
  type: oauth2
slug: microsoft-azure-openai-authentication
source_filename: microsoft-azure-openai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/microsoft-azure-openai-batch-api-openapi.yml, openapi/microsoft-azure-openai-deployments-api-openapi.yml,\n  openapi/microsoft-azure-openai-files-api-openapi.yml, openapi/microsoft-azure-openai-fine-tuning-api-openapi.yml,\n  openapi/microsoft-azure-openai-models-api-openapi.yml, openapi/microsoft-azure-openai-uploadfile-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Provide your Cognitive Services Azure OpenAI account key here.\n  sources:\n  - openapi/microsoft-azure-openai-batch-api-openapi.yml\n  - openapi/microsoft-azure-openai-deployments-api-openapi.yml\n  - openapi/microsoft-azure-openai-files-api-openapi.yml\n  - openapi/microsoft-azure-openai-fine-tuning-api-openapi.yml\n  - openapi/microsoft-azure-openai-models-api-openapi.yml\n  - openapi/microsoft-azure-openai-uploadfile-api-openapi.yml\n\
  - name: bearer\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    scopes: 0\n  sources:\n  - openapi/microsoft-azure-openai-deployments-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-openai/authentication/microsoft-azure-openai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Embeddings
- GPT
- Generative AI
- LLM
- OpenAI
---
