---
api_key_in: []
api_specs:
- filename: keywordsai-datasets-api-openapi.yml
  format: yaml
  label: Keywords AI Datasets API
  slug: keywordsai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-datasets-api-openapi.yml
- filename: keywordsai-evaluators-api-openapi.yml
  format: yaml
  label: Keywords AI Evaluators API
  slug: keywordsai-evaluators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-evaluators-api-openapi.yml
- filename: keywordsai-experiments-api-openapi.yml
  format: yaml
  label: Keywords AI Experiments API
  slug: keywordsai-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-experiments-api-openapi.yml
- filename: keywordsai-gateway-api-openapi.yml
  format: yaml
  label: Keywords AI Gateway API
  slug: keywordsai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-gateway-api-openapi.yml
- filename: keywordsai-logging-api-openapi.yml
  format: yaml
  label: Keywords AI Logging API
  slug: keywordsai-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-logging-api-openapi.yml
- filename: keywordsai-prompts-api-openapi.yml
  format: yaml
  label: Keywords AI Prompts API
  slug: keywordsai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-prompts-api-openapi.yml
- filename: keywordsai-threads-api-openapi.yml
  format: yaml
  label: Keywords AI Threads API
  slug: keywordsai-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-threads-api-openapi.yml
- filename: keywordsai-traces-api-openapi.yml
  format: yaml
  label: Keywords AI Traces API
  slug: keywordsai-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-traces-api-openapi.yml
- filename: keywordsai-users-api-openapi.yml
  format: yaml
  label: Keywords AI Users API
  slug: keywordsai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keywordsai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keywords AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keywords AI
provider_slug: keywordsai
scheme_count: 1
schemes:
- description: 'Keywords AI API key supplied as the Authorization Bearer header (Authorization: Bearer <KEYWORDSAI_API_KEY>).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keywordsai-openapi.yml
  type: http
slug: keywordsai-authentication
source_filename: keywordsai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keywordsai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Keywords AI API key supplied as the Authorization Bearer header (Authorization:\n    Bearer <KEYWORDSAI_API_KEY>).'\n  sources:\n  - openapi/keywordsai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/authentication/keywordsai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Observability
- Gateway
- Monitoring
---
