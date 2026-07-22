---
api_key_in: []
api_specs:
- filename: recursal-ai-inc-featherless-openapi.yml
  format: yaml
  label: Featherless AI Serverless Inference API
  slug: featherless-ai-serverless-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recursal-ai-inc/refs/heads/main/openapi/recursal-ai-inc-featherless-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Recursal Ai Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recursal AI, Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recursal AI, Inc.
provider_slug: recursal-ai-inc
scheme_count: 1
schemes:
- description: 'Featherless API key supplied as an HTTP Bearer token (Authorization: Bearer FEATHERLESS_API_KEY). Keys are created in account settings.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/recursal-ai-inc-featherless-openapi.yml
  type: http
slug: recursal-ai-inc-authentication
source_filename: recursal-ai-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/recursal-ai-inc-featherless-openapi.yml\ndocs: https://featherless.ai/docs/quickstart-guide\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Featherless API key supplied as an HTTP Bearer token (Authorization: Bearer\n    FEATHERLESS_API_KEY). Keys are created in account settings.'\n  sources:\n  - openapi/recursal-ai-inc-featherless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recursal-ai-inc/refs/heads/main/authentication/recursal-ai-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Serverless
- Generative AI
- Developer Tools
- OpenAI Compatible
- RWKV
---
