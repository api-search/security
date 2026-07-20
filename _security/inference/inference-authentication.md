---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Inference Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inference secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inference
provider_slug: inference
scheme_count: 1
schemes:
- base_url: https://api.inference.net/v1
  description: Pass the project API key as a Bearer token in the Authorization header. Keys are project-scoped and carry read/write permission levels. The API is OpenAI-compatible, so the same key works with the OpenAI SDK by setting base_url to https://api.inference.net/v1.
  env: INFERENCE_API_KEY
  format: 'Authorization: Bearer <api-key>'
  header: Authorization
  in: header
  name: apiKey
  scheme: bearer
  type: http
slug: inference-authentication
source_filename: inference-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.inference.net/reference/api-keys\ndocs: https://docs.inference.net/reference/api-keys\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Authorization: Bearer <api-key>\"\n  env: INFERENCE_API_KEY\n  base_url: https://api.inference.net/v1\n  description: >-\n    Pass the project API key as a Bearer token in the Authorization header. Keys are\n    project-scoped and carry read/write permission levels. The API is OpenAI-compatible,\n    so the same key works with the OpenAI SDK by setting base_url to\n    https://api.inference.net/v1.\nnotes:\n- Keys are managed in the dashboard, scoped per project, with read/write permissions.\n- The hosted MCP server (https://mcp.inference.net/mcp) uses the same Bearer project key.\n- CLI (`inf`) supports interactive sign-in and API-key auth for CI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inference/refs/heads/main/authentication/inference-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Observability
- Model Training
- Model Deployment
- MCP
- Crypto Web3
---
