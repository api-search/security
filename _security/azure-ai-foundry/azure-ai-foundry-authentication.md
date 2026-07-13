---
api_key_in:
- header
api_specs:
- filename: azure-ai-foundry-openapi.yml
  format: yaml
  label: Azure AI Foundry REST API
  slug: foundry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Ai Foundry Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Microsoft Azure AI Foundry secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Microsoft Azure AI Foundry
provider_slug: azure-ai-foundry
scheme_count: 2
schemes:
- description: Foundry/Azure OpenAI resource API key
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/azure-ai-foundry-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://ai.azure.com/.default)
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-ai-foundry-openapi.yml
  type: oauth2
slug: azure-ai-foundry-authentication
source_filename: azure-ai-foundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-ai-foundry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Foundry/Azure OpenAI resource API key\n  sources:\n  - openapi/azure-ai-foundry-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://ai.azure.com/.default)\n  sources:\n  - openapi/azure-ai-foundry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/authentication/azure-ai-foundry-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Generative AI
- AI Agents
- Foundation Models
- Machine Learning
- Cloud
- Azure
---
