---
api_key_in: []
api_specs:
- filename: meilisearch-documents-api-openapi.yml
  format: yaml
  label: Meilisearch Documents API
  slug: meilisearch-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-documents-api-openapi.yml
- filename: meilisearch-health-api-openapi.yml
  format: yaml
  label: Meilisearch Health API
  slug: meilisearch-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-health-api-openapi.yml
- filename: meilisearch-indexes-api-openapi.yml
  format: yaml
  label: Meilisearch Indexes API
  slug: meilisearch-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-indexes-api-openapi.yml
- filename: meilisearch-keys-api-openapi.yml
  format: yaml
  label: Meilisearch Keys API
  slug: meilisearch-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-keys-api-openapi.yml
- filename: meilisearch-search-api-openapi.yml
  format: yaml
  label: Meilisearch Search API
  slug: meilisearch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-search-api-openapi.yml
- filename: meilisearch-settings-api-openapi.yml
  format: yaml
  label: Meilisearch Settings API
  slug: meilisearch-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-settings-api-openapi.yml
- filename: meilisearch-tasks-api-openapi.yml
  format: yaml
  label: Meilisearch Tasks API
  slug: meilisearch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meilisearch/refs/heads/main/openapi/meilisearch-tasks-api-openapi.yml
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
- Open-Source
- Search
---
