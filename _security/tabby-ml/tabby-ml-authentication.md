---
api_key_in: []
api_specs:
- filename: tabby-ml-chat-api-openapi.yml
  format: yaml
  label: Tabby Chat API
  slug: tabby-ml-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-chat-api-openapi.yml
- filename: tabby-ml-completions-api-openapi.yml
  format: yaml
  label: Tabby Completions API
  slug: tabby-ml-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-completions-api-openapi.yml
- filename: tabby-ml-events-api-openapi.yml
  format: yaml
  label: Tabby Events API
  slug: tabby-ml-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-events-api-openapi.yml
- filename: tabby-ml-health-api-openapi.yml
  format: yaml
  label: Tabby Health API
  slug: tabby-ml-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-health-api-openapi.yml
- filename: tabby-ml-ingestion-api-openapi.yml
  format: yaml
  label: Tabby Ingestion API
  slug: tabby-ml-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-ingestion-api-openapi.yml
- filename: tabby-ml-models-api-openapi.yml
  format: yaml
  label: Tabby Models API
  slug: tabby-ml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tabby Ml Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabby secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tabby
provider_slug: tabby-ml
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Tabby uses a registration token from the self-hosted web UI (Information -> System -> Registration token), passed as `Authorization: Bearer [example key]`. Because Tabby is self-hosted, tokens are minted by your own instance rather than a central vendor console.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tabby-ml-openapi.yml
  - https://www.tabbyml.com/blog/doc-ingestion-api
  type: http
slug: tabby-ml-authentication
source_filename: tabby-ml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tabby-ml-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication. Tabby uses a registration token from the\n    self-hosted web UI (Information -> System -> Registration token), passed as `Authorization:\n    Bearer [example key]`. Because Tabby is self-hosted, tokens are minted by your own\n    instance rather than a central vendor console.'\n  sources:\n  - openapi/tabby-ml-openapi.yml\n  - https://www.tabbyml.com/blog/doc-ingestion-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/authentication/tabby-ml-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Coding Assistant
- Code Completion
- Open-Source
- Developer Tools
- LLM
- Artificial Intelligence
- Self-Hosted
- Code Generation
- Copilot Alternative
---
