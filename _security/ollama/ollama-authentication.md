---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Ollama API
  slug: ollama-api
  spec_type: OpenAPI
  url: https://docs.ollama.com/openapi.yaml
- filename: ollama-openai-compatibility-api-openapi.yml
  format: yaml
  label: Ollama OpenAI Compatibility API
  slug: ollama-openai-compatibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-openai-compatibility-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ollama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ollama secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ollama
provider_slug: ollama
scheme_count: 1
schemes:
- description: API key authentication. The key is accepted but not validated by Ollama. Use any value such as ollama.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ollama-openai-compatibility-api-openapi.yml
  type: http
slug: ollama-authentication
source_filename: ollama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ollama-openai-compatibility-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication. The key is accepted but not validated by Ollama. Use\n    any value such as ollama.\n  sources:\n  - openapi/ollama-openai-compatibility-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/authentication/ollama-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Large Language Models
- Models
---
