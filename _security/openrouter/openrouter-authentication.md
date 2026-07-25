---
api_key_in: []
api_specs:
- filename: openrouter-chat-api-openapi.yml
  format: yaml
  label: OpenRouter Chat API
  slug: openrouter-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-chat-api-openapi.yml
- filename: openrouter-completions-api-openapi.yml
  format: yaml
  label: OpenRouter Completions API
  slug: openrouter-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-completions-api-openapi.yml
- filename: openrouter-credits-api-openapi.yml
  format: yaml
  label: OpenRouter Credits API
  slug: openrouter-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-credits-api-openapi.yml
- filename: openrouter-generation-api-openapi.yml
  format: yaml
  label: OpenRouter Generation API
  slug: openrouter-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-generation-api-openapi.yml
- filename: openrouter-keys-api-openapi.yml
  format: yaml
  label: OpenRouter Keys API
  slug: openrouter-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-keys-api-openapi.yml
- filename: openrouter-models-api-openapi.yml
  format: yaml
  label: OpenRouter Models API
  slug: openrouter-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-models-api-openapi.yml
- filename: openrouter-providers-api-openapi.yml
  format: yaml
  label: OpenRouter Providers API
  slug: openrouter-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-providers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openrouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRouter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRouter
provider_slug: openrouter
scheme_count: 1
schemes:
- bearerFormat: OPENROUTER_API_KEY
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openrouter-openapi.yml
  type: http
slug: openrouter-authentication
source_filename: openrouter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openrouter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OPENROUTER_API_KEY\n  sources:\n  - openapi/openrouter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/authentication/openrouter-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Gateway
- Large Language Models
- Router
---
