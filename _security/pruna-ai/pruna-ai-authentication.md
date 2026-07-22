---
api_key_in:
- header
api_specs:
- filename: pruna-ai-openapi.yml
  format: yaml
  label: Pruna P-API
  slug: pruna-p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pruna-ai/refs/heads/main/openapi/pruna-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pruna Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pruna AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pruna AI
provider_slug: pruna-ai
scheme_count: 1
schemes:
- description: 'API key for authentication. You can obtain your API key from the

    Pruna AI dashboard.


    Include it in the `apikey` header for all requests.'
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/pruna-ai-openapi.yml
  type: apiKey
slug: pruna-ai-authentication
source_filename: pruna-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pruna-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: |-\n    API key for authentication. You can obtain your API key from the\n    Pruna AI dashboard.\n\n    Include it in the `apikey` header for all requests.\n  sources:\n  - openapi/pruna-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pruna-ai/refs/heads/main/authentication/pruna-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Generation
- Video Generation
- Generative AI
- Model Optimization
- Inference
- Developer Tools
---
