---
api_key_in:
- header
api_specs:
- filename: miriel-documents-api-openapi.yml
  format: yaml
  label: Miriel Documents API
  slug: miriel-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-documents-api-openapi.yml
- filename: miriel-learn-api-openapi.yml
  format: yaml
  label: Miriel Learn API
  slug: miriel-learn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-learn-api-openapi.yml
- filename: miriel-monitoring-api-openapi.yml
  format: yaml
  label: Miriel Monitoring API
  slug: miriel-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-monitoring-api-openapi.yml
- filename: miriel-policies-api-openapi.yml
  format: yaml
  label: Miriel Policies API
  slug: miriel-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-policies-api-openapi.yml
- filename: miriel-projects-api-openapi.yml
  format: yaml
  label: Miriel Projects API
  slug: miriel-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-projects-api-openapi.yml
- filename: miriel-query-api-openapi.yml
  format: yaml
  label: Miriel Query API
  slug: miriel-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-query-api-openapi.yml
- filename: miriel-users-api-openapi.yml
  format: yaml
  label: Miriel Users API
  slug: miriel-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/openapi/miriel-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Miriel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Miriel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Miriel
provider_slug: miriel
scheme_count: 1
schemes:
- description: API key issued from the Miriel dashboard, sent in the x-access-token header.
  in: header
  name: accessToken
  parameter: x-access-token
  sources:
  - openapi/miriel-openapi.yml
  type: apiKey
slug: miriel-authentication
source_filename: miriel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/miriel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-access-token\n  description: API key issued from the Miriel dashboard, sent in the x-access-token header.\n  sources:\n  - openapi/miriel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miriel/refs/heads/main/authentication/miriel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Context Engine
- Retrieval
- RAG
- Knowledge Graph
- Vector Search
- Agents
- LLM
- Developer Tools
---
