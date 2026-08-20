---
api_key_in:
- header
- query
api_specs:
- filename: vast-ai-accounts-api-openapi.yml
  format: yaml
  label: Vast.ai Accounts API
  slug: vast-ai-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-accounts-api-openapi.yml
- filename: vast-ai-billing-api-openapi.yml
  format: yaml
  label: Vast.ai Billing API
  slug: vast-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-billing-api-openapi.yml
- filename: vast-ai-instances-api-openapi.yml
  format: yaml
  label: Vast.ai Instances API
  slug: vast-ai-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-instances-api-openapi.yml
- filename: vast-ai-machines-api-openapi.yml
  format: yaml
  label: Vast.ai Machines API
  slug: vast-ai-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-machines-api-openapi.yml
- filename: vast-ai-network-volumes-api-openapi.yml
  format: yaml
  label: Vast.ai Network Volumes API
  slug: vast-ai-network-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-network-volumes-api-openapi.yml
- filename: vast-ai-search-api-openapi.yml
  format: yaml
  label: Vast.ai Search API
  slug: vast-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-search-api-openapi.yml
- filename: vast-ai-serverless-api-openapi.yml
  format: yaml
  label: Vast.ai Serverless API
  slug: vast-ai-serverless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-serverless-api-openapi.yml
- filename: vast-ai-team-api-openapi.yml
  format: yaml
  label: Vast.ai Team API
  slug: vast-ai-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-team-api-openapi.yml
- filename: vast-ai-templates-api-openapi.yml
  format: yaml
  label: Vast.ai Templates API
  slug: vast-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-templates-api-openapi.yml
- filename: vast-ai-volumes-api-openapi.yml
  format: yaml
  label: Vast.ai Volumes API
  slug: vast-ai-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-volumes-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vast Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vast.ai secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vast.ai
provider_slug: vast-ai
scheme_count: 3
schemes:
- description: API key authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vast-ai-openapi.json
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/vast-ai-openapi.json
  type: apiKey
- description: API key must be provided as a query parameter
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/vast-ai-openapi.json
  type: apiKey
slug: vast-ai-authentication
source_filename: vast-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vast-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication\n  sources:\n  - openapi/vast-ai-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/vast-ai-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key must be provided as a query parameter\n  sources:\n  - openapi/vast-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/authentication/vast-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artificial Intelligence
- Cloud
- Compute
- GPU
- Machine-Learning
- Marketplace
- Serverless
---
