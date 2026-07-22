---
api_key_in:
- header
api_specs:
- filename: unitlab-ai-sdk-openapi.yml
  format: yaml
  label: Unitlab SDK API
  slug: unitlab-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitlab-ai/refs/heads/main/openapi/unitlab-ai-sdk-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unitlab Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unitlab AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unitlab AI
provider_slug: unitlab-ai
scheme_count: 1
schemes:
- description: 'API key issued at https://app.unitlab.ai (API Keys page), sent as "Authorization: Api-Key <key>". The SDK/CLI also read UNITLAB_API_KEY or ~/.unitlab/credentials.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/unitlab-ai-sdk-openapi.yml
  type: apiKey
slug: unitlab-ai-authentication
source_filename: unitlab-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unitlab-ai-sdk-openapi.yml\ndocs: https://docs.unitlab.ai/how-to-integrate/create-an-api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key issued at https://app.unitlab.ai (API Keys page), sent as \"Authorization:\n    Api-Key <key>\". The SDK/CLI also read UNITLAB_API_KEY or ~/.unitlab/credentials.'\n  sources:\n  - openapi/unitlab-ai-sdk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitlab-ai/refs/heads/main/authentication/unitlab-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Annotation
- Machine Learning
- Computer Vision
- Datasets
- Artificial Intelligence
- Labeling
---
