---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Knowledge Graph Search API
  slug: google-knowledge-graph-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-knowledge-graph/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Google Knowledge Graph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Knowledge Graph Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google Knowledge Graph Search
provider_slug: google-knowledge-graph
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: google-knowledge-graph-authentication
source_filename: google-knowledge-graph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-knowledge-graph/refs/heads/main/authentication/google-knowledge-graph-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entities
- Google
- Knowledge Graph
- Linked Data
- Schema.org
- Semantic Search
---
