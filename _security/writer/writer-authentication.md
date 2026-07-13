---
api_key_in: []
api_specs:
- filename: writer-openapi.yml
  format: yaml
  label: Writer Chat Completion API
  slug: writer-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Text Generation API
  slug: writer-text-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Tool Calling API
  slug: writer-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Knowledge Graph API
  slug: writer-knowledge-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Files API
  slug: writer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Applications API
  slug: writer-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Vision API
  slug: writer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Web Search API
  slug: writer-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Translation API
  slug: writer-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Models API
  slug: writer-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Guardrails API
  slug: writer-guardrails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer API Keys API
  slug: writer-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Writer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Writer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Writer
provider_slug: writer
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is your [Writer API key](https://dev.writer.com/api-reference/api-keys).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/writer-openapi.yml
  type: http
slug: writer-authentication
source_filename: writer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/writer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is\n    your [Writer API key](https://dev.writer.com/api-reference/api-keys).\n  sources:\n  - openapi/writer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/authentication/writer-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Enterprise
- Content Generation
- Palmyra
- Agents
---
