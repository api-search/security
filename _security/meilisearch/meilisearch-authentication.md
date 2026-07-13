---
api_key_in: []
api_specs:
- filename: meilisearch-openapi.yml
  format: yaml
  label: Meilisearch API
  slug: meilisearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Meilisearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meilisearch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meilisearch
provider_slug: meilisearch
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'Authorization header using "Authorization: Bearer {API_KEY}".

    The master key authorizes /keys management; regular API keys

    should be used for all other routes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/meilisearch-openapi.yml
  type: http
slug: meilisearch-authentication
source_filename: meilisearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meilisearch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: |-\n    Authorization header using \"Authorization: Bearer {API_KEY}\".\n    The master key authorizes /keys management; regular API keys\n    should be used for all other routes.\n  sources:\n  - openapi/meilisearch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/authentication/meilisearch-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Search
- Full-Text Search
- Hybrid Search
- Open Source
- Search
---
