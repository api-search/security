---
api_key_in:
- header
api_specs:
- filename: searchcraft-authentication-api-openapi.yml
  format: yaml
  label: Searchcraft Authentication API
  slug: searchcraft-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-authentication-api-openapi.yml
- filename: searchcraft-documents-api-openapi.yml
  format: yaml
  label: Searchcraft Documents API
  slug: searchcraft-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-documents-api-openapi.yml
- filename: searchcraft-federation-api-openapi.yml
  format: yaml
  label: Searchcraft Federation API
  slug: searchcraft-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-federation-api-openapi.yml
- filename: searchcraft-healthcheck-api-openapi.yml
  format: yaml
  label: Searchcraft Healthcheck API
  slug: searchcraft-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-healthcheck-api-openapi.yml
- filename: searchcraft-indexes-api-openapi.yml
  format: yaml
  label: Searchcraft Indexes API
  slug: searchcraft-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-indexes-api-openapi.yml
- filename: searchcraft-measure-api-openapi.yml
  format: yaml
  label: Searchcraft Measure API
  slug: searchcraft-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-measure-api-openapi.yml
- filename: searchcraft-search-api-openapi.yml
  format: yaml
  label: Searchcraft Search API
  slug: searchcraft-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-search-api-openapi.yml
- filename: searchcraft-stopwords-api-openapi.yml
  format: yaml
  label: Searchcraft Stopwords API
  slug: searchcraft-stopwords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-stopwords-api-openapi.yml
- filename: searchcraft-synonyms-api-openapi.yml
  format: yaml
  label: Searchcraft Synonyms API
  slug: searchcraft-synonyms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-synonyms-api-openapi.yml
- filename: searchcraft-transactions-api-openapi.yml
  format: yaml
  label: Searchcraft Transactions API
  slug: searchcraft-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-transactions-api-openapi.yml
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
