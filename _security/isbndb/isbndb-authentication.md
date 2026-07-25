---
api_key_in:
- header
api_specs:
- filename: isbndb-author-api-openapi.yml
  format: yaml
  label: ISBNdb Author API
  slug: isbndb-author-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-author-api-openapi.yml
- filename: isbndb-books-api-openapi.yml
  format: yaml
  label: ISBNdb Books API
  slug: isbndb-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-books-api-openapi.yml
- filename: isbndb-feed-api-openapi.yml
  format: yaml
  label: ISBNdb Feed API
  slug: isbndb-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-feed-api-openapi.yml
- filename: isbndb-key-api-openapi.yml
  format: yaml
  label: ISBNdb Key API
  slug: isbndb-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-key-api-openapi.yml
- filename: isbndb-publisher-api-openapi.yml
  format: yaml
  label: ISBNdb Publisher API
  slug: isbndb-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-publisher-api-openapi.yml
- filename: isbndb-search-api-openapi.yml
  format: yaml
  label: ISBNdb Search API
  slug: isbndb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-search-api-openapi.yml
- filename: isbndb-stats-api-openapi.yml
  format: yaml
  label: ISBNdb Stats API
  slug: isbndb-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-stats-api-openapi.yml
- filename: isbndb-subject-api-openapi.yml
  format: yaml
  label: ISBNdb Subject API
  slug: isbndb-subject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/openapi/isbndb-subject-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Isbndb Authentication
name_suffix: Authentication
oauth_flows: []
overview: ISBNdb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ISBNdb
provider_slug: isbndb
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
slug: isbndb-authentication
source_filename: isbndb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/authentication/isbndb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Books
- ISBN
- Publishing
- Metadata
- Library
- Bibliography
---
