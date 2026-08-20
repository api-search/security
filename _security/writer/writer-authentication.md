---
api_key_in: []
api_specs:
- filename: writer-file-api-api-openapi.yml
  format: yaml
  label: Writer File API API
  slug: writer-file-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-file-api-api-openapi.yml
- filename: writer-generation-api-api-openapi.yml
  format: yaml
  label: Writer Generation API API
  slug: writer-generation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-generation-api-api-openapi.yml
- filename: writer-kg-api-api-openapi.yml
  format: yaml
  label: Writer KG API API
  slug: writer-kg-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-kg-api-api-openapi.yml
- filename: writer-template-api-openapi.yml
  format: yaml
  label: Writer template API
  slug: writer-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-template-api-openapi.yml
- filename: writer-tools-api-api-openapi.yml
  format: yaml
  label: Writer Tools API API
  slug: writer-tools-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-tools-api-api-openapi.yml
- filename: writer-translation-api-openapi.yml
  format: yaml
  label: Writer Translation API
  slug: writer-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-translation-api-openapi.yml
- filename: writer-vision-api-openapi.yml
  format: yaml
  label: Writer Vision API
  slug: writer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-vision-api-openapi.yml
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
- Artificial Intelligence
- LLM
- Enterprise
- Content Generation
- Palmyra
- Agents
---
