---
api_key_in:
- header
api_specs:
- filename: elastic-search-cat-api-openapi.yml
  format: yaml
  label: Elasticsearch Cat API
  slug: elastic-search-cat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/openapi/elastic-search-cat-api-openapi.yml
- filename: elastic-search-cluster-api-openapi.yml
  format: yaml
  label: Elasticsearch Cluster API
  slug: elastic-search-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/openapi/elastic-search-cluster-api-openapi.yml
- filename: elastic-search-document-api-openapi.yml
  format: yaml
  label: Elasticsearch Document API
  slug: elastic-search-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/openapi/elastic-search-document-api-openapi.yml
- filename: elastic-search-index-api-openapi.yml
  format: yaml
  label: Elasticsearch Index API
  slug: elastic-search-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/openapi/elastic-search-index-api-openapi.yml
- filename: elastic-search-search-api-openapi.yml
  format: yaml
  label: Elasticsearch Search API
  slug: elastic-search-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/openapi/elastic-search-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elasticsearch secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elasticsearch
provider_slug: elastic-search
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elastic-search-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elastic-search-openapi.yml
  type: apiKey
slug: elastic-search-authentication
source_filename: elastic-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elastic-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elastic-search-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/elastic-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/authentication/elastic-search-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Database
- Distributed Systems
- Full-Text Search
- NoSQL
- Search
---
