---
api_key_in: []
api_specs:
- filename: client
  format: yaml
  label: Glean Client API
  slug: glean-client-api
  spec_type: OpenAPI
  url: https://developers.glean.com/oas/client
- filename: indexing
  format: yaml
  label: Glean Indexing API
  slug: glean-indexing-api
  spec_type: OpenAPI
  url: https://developers.glean.com/oas/indexing
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glean Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glean secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glean
provider_slug: glean
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Glean API token, passed as `Authorization: Bearer <token>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/glean-openapi.yml
  type: http
slug: glean-authentication
source_filename: glean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glean-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Glean API token, passed as `Authorization: Bearer <token>`'\n  sources:\n  - openapi/glean-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/authentication/glean-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- AI
- Answers
- Chat
- Connectors
- Enterprise Search
- Generative AI
- Indexing
- Knowledge
- RAG
- Search
- Work Assistant
---
