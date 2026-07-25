---
api_key_in: []
api_specs:
- filename: unify-ai-agent-api-openapi.yml
  format: yaml
  label: Unify Agent API
  slug: unify-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-agent-api-openapi.yml
- filename: unify-ai-assistants-api-openapi.yml
  format: yaml
  label: Unify Assistants API
  slug: unify-ai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-assistants-api-openapi.yml
- filename: unify-ai-contexts-api-openapi.yml
  format: yaml
  label: Unify Contexts API
  slug: unify-ai-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-contexts-api-openapi.yml
- filename: unify-ai-logs-api-openapi.yml
  format: yaml
  label: Unify Logs API
  slug: unify-ai-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-logs-api-openapi.yml
- filename: unify-ai-organizations-api-openapi.yml
  format: yaml
  label: Unify Organizations API
  slug: unify-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-organizations-api-openapi.yml
- filename: unify-ai-platform-api-openapi.yml
  format: yaml
  label: Unify Platform API
  slug: unify-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-platform-api-openapi.yml
- filename: unify-ai-projects-api-openapi.yml
  format: yaml
  label: Unify Projects API
  slug: unify-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-projects-api-openapi.yml
- filename: unify-ai-spaces-api-openapi.yml
  format: yaml
  label: Unify Spaces API
  slug: unify-ai-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-spaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unify Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unify
provider_slug: unify-ai
scheme_count: 1
schemes:
- description: API key from the Unify console (UNIFY_KEY environment variable)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unify-ai-universal-api-openapi.yml
  type: http
slug: unify-ai-authentication
source_filename: unify-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unify-ai-universal-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from the Unify console (UNIFY_KEY environment variable)\n  sources:\n  - openapi/unify-ai-universal-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/authentication/unify-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- LLM
- AI
- Large Language Models
- LLM Routing
- Model Gateway
- AI Gateway
- OpenAI
- Anthropic
- Mistral
- Benchmarking
- Model Comparison
- AI Infrastructure
- Machine Learning
---
