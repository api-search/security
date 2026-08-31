---
api_key_in: []
api_specs:
- filename: cerebras-systems-chat-api-openapi.yml
  format: yaml
  label: Cerebras Systems Chat API
  slug: cerebras-systems-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/openapi/cerebras-systems-chat-api-openapi.yml
- filename: cerebras-systems-completions-api-openapi.yml
  format: yaml
  label: Cerebras Systems Completions API
  slug: cerebras-systems-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/openapi/cerebras-systems-completions-api-openapi.yml
- filename: cerebras-systems-models-api-openapi.yml
  format: yaml
  label: Cerebras Systems Models API
  slug: cerebras-systems-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/openapi/cerebras-systems-models-api-openapi.yml
- filename: cerebras-systems-public-models-api-openapi.yml
  format: yaml
  label: Cerebras Systems Public Models API
  slug: cerebras-systems-public-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/openapi/cerebras-systems-public-models-api-openapi.yml
- filename: cerebras-systems-tcp-warming-api-openapi.yml
  format: yaml
  label: Cerebras Systems Tcp Warming API
  slug: cerebras-systems-tcp-warming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/openapi/cerebras-systems-tcp-warming-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cerebras Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerebras Systems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cerebras Systems
provider_slug: cerebras-systems
scheme_count: 1
schemes:
- description: 'API key for authentication. Obtain your key from the Cerebras Cloud console and pass it as `Authorization: Bearer [example key]`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cerebras-systems-chat-completions-openapi.yaml
  - openapi/cerebras-systems-inference-openapi-original.yml
  type: http
slug: cerebras-systems-authentication
source_filename: cerebras-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cerebras-systems-chat-completions-openapi.yaml, openapi/cerebras-systems-inference-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key for authentication. Obtain your key from the Cerebras Cloud console\n    and pass it as `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/cerebras-systems-chat-completions-openapi.yaml\n  - openapi/cerebras-systems-inference-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebras-systems/refs/heads/main/authentication/cerebras-systems-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Infrastructure
- Artificial Intelligence
- Machine-Learning
- Inference
- Large Language Models
- Developer Tools
- Cloud Computing
- Semiconductors
---
