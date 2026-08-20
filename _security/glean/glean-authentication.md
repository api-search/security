---
api_key_in: []
api_specs:
- filename: glean-search-api-openapi.yml
  format: yaml
  label: Glean Search API
  slug: glean-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-search-api-openapi.yml
- filename: glean-chat-api-openapi.yml
  format: yaml
  label: Glean Chat API
  slug: glean-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-chat-api-openapi.yml
- filename: glean-agents-api-openapi.yml
  format: yaml
  label: Glean Agents API
  slug: glean-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-agents-api-openapi.yml
- filename: glean-people-api-openapi.yml
  format: yaml
  label: Glean People API
  slug: glean-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-people-api-openapi.yml
- filename: glean-activity-api-openapi.yml
  format: yaml
  label: Glean Activity API
  slug: glean-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-activity-api-openapi.yml
- filename: glean-governance-api-openapi.yml
  format: yaml
  label: Glean Governance API
  slug: glean-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-governance-api-openapi.yml
- filename: glean-activity-api-openapi.yml
  format: yaml
  label: Glean activity API
  slug: glean-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-activity-api-openapi.yml
- filename: glean-agents-api-openapi.yml
  format: yaml
  label: Glean agents API
  slug: glean-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-agents-api-openapi.yml
- filename: glean-announcements-api-openapi.yml
  format: yaml
  label: Glean announcements API
  slug: glean-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-announcements-api-openapi.yml
- filename: glean-answers-api-openapi.yml
  format: yaml
  label: Glean answers API
  slug: glean-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-answers-api-openapi.yml
- filename: glean-chat-api-openapi.yml
  format: yaml
  label: Glean chat API
  slug: glean-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-chat-api-openapi.yml
- filename: glean-collections-api-openapi.yml
  format: yaml
  label: Glean collections API
  slug: glean-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-collections-api-openapi.yml
- filename: glean-documents-api-openapi.yml
  format: yaml
  label: Glean documents API
  slug: glean-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-documents-api-openapi.yml
- filename: glean-governance-api-openapi.yml
  format: yaml
  label: Glean governance API
  slug: glean-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-governance-api-openapi.yml
- filename: glean-insights-api-openapi.yml
  format: yaml
  label: Glean insights API
  slug: glean-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-insights-api-openapi.yml
- filename: glean-people-api-openapi.yml
  format: yaml
  label: Glean people API
  slug: glean-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-people-api-openapi.yml
- filename: glean-pins-api-openapi.yml
  format: yaml
  label: Glean pins API
  slug: glean-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-pins-api-openapi.yml
- filename: glean-search-api-openapi.yml
  format: yaml
  label: Glean search API
  slug: glean-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-search-api-openapi.yml
- filename: glean-shortcuts-api-openapi.yml
  format: yaml
  label: Glean shortcuts API
  slug: glean-shortcuts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-shortcuts-api-openapi.yml
- filename: glean-summarize-api-openapi.yml
  format: yaml
  label: Glean summarize API
  slug: glean-summarize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-summarize-api-openapi.yml
- filename: glean-tools-api-openapi.yml
  format: yaml
  label: Glean tools API
  slug: glean-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-tools-api-openapi.yml
- filename: glean-verification-api-openapi.yml
  format: yaml
  label: Glean verification API
  slug: glean-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-verification-api-openapi.yml
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
- Artificial Intelligence
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
