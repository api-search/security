---
api_key_in:
- header
api_specs:
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Index API
  slug: searchcraft-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Documents / Ingest API
  slug: searchcraft-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Search API
  slug: searchcraft-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Federated Search API
  slug: searchcraft-federated-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Synonyms & Stopwords API
  slug: searchcraft-synonyms-stopwords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Searchcraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Searchcraft secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Searchcraft
provider_slug: searchcraft
scheme_count: 1
schemes:
- description: 'Searchcraft access key passed directly in the Authorization header (no "Bearer" prefix). Keys are tiered by permission: read (search), ingest (document, synonym, stopword, transaction, and measure writes), and admin (index, federation, and key management). Keys may be scoped to specific indexes via allowed_indexes.'
  in: header
  name: SearchcraftKey
  parameter: Authorization
  sources:
  - openapi/searchcraft-openapi.yml
  type: apiKey
slug: searchcraft-authentication
source_filename: searchcraft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/searchcraft-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SearchcraftKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Searchcraft access key passed directly in the Authorization header (no \"Bearer\"\n    prefix). Keys are tiered by permission: read (search), ingest (document, synonym, stopword,\n    transaction, and measure writes), and admin (index, federation, and key management). Keys\n    may be scoped to specific indexes via allowed_indexes.'\n  sources:\n  - openapi/searchcraft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/authentication/searchcraft-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- Search as a Service
- Full Text Search
- Indexing
- Developer Tools
---
