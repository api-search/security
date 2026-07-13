---
api_key_in: []
api_specs:
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Apps and Variants API
  slug: agenta-apps-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Configs and Prompts API
  slug: agenta-configs-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Evaluations and Evaluators API
  slug: agenta-evaluations-evaluators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Testsets API
  slug: agenta-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Observability and Traces API
  slug: agenta-observability-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agenta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agenta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agenta
provider_slug: agenta
scheme_count: 1
schemes:
- description: 'Agenta API key sent in the Authorization header. Generate keys from the Agenta web app under Settings > API keys. The value is passed as `Authorization: ApiKey <key>` (Bearer-style header credential).'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/agenta-openapi.yml
  type: http
slug: agenta-authentication
source_filename: agenta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agenta-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Agenta API key sent in the Authorization header. Generate keys from the Agenta\n    web app under Settings > API keys. The value is passed as `Authorization: ApiKey <key>`\n    (Bearer-style header credential).'\n  sources:\n  - openapi/agenta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/authentication/agenta-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLMOps
- Prompt Management
- LLM Evaluation
- Observability
---
