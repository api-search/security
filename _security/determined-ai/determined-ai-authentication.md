---
api_key_in: []
api_specs:
- filename: determined-ai-authentication-api-openapi.yml
  format: yaml
  label: Determined AI Authentication API
  slug: determined-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-authentication-api-openapi.yml
- filename: determined-ai-checkpoints-api-openapi.yml
  format: yaml
  label: Determined AI Checkpoints API
  slug: determined-ai-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-checkpoints-api-openapi.yml
- filename: determined-ai-cluster-api-openapi.yml
  format: yaml
  label: Determined AI Cluster API
  slug: determined-ai-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-cluster-api-openapi.yml
- filename: determined-ai-experiments-api-openapi.yml
  format: yaml
  label: Determined AI Experiments API
  slug: determined-ai-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-experiments-api-openapi.yml
- filename: determined-ai-models-api-openapi.yml
  format: yaml
  label: Determined AI Models API
  slug: determined-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-models-api-openapi.yml
- filename: determined-ai-templates-api-openapi.yml
  format: yaml
  label: Determined AI Templates API
  slug: determined-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-templates-api-openapi.yml
- filename: determined-ai-tokens-api-openapi.yml
  format: yaml
  label: Determined AI Tokens API
  slug: determined-ai-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-tokens-api-openapi.yml
- filename: determined-ai-users-api-openapi.yml
  format: yaml
  label: Determined AI Users API
  slug: determined-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/openapi/determined-ai-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Determined Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Determined AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Determined AI
provider_slug: determined-ai
scheme_count: 1
schemes:
- description: Bearer token issued by the /auth/login endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/determined-ai-openapi.yml
  type: http
slug: determined-ai-authentication
source_filename: determined-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/determined-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued by the /auth/login endpoint.\n  sources:\n  - openapi/determined-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/determined-ai/refs/heads/main/authentication/determined-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Deep Learning
- Machine Learning
- MLOps
---
