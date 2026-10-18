---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zincsearch-document-api-openapi.yml
  format: yaml
  label: ZincSearch Document API
  slug: zincsearch-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-document-api-openapi.yml
- filename: zincsearch-healthz-api-openapi.yml
  format: yaml
  label: ZincSearch Healthz API
  slug: zincsearch-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-healthz-api-openapi.yml
- filename: zincsearch-index-api-openapi.yml
  format: yaml
  label: ZincSearch Index API
  slug: zincsearch-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-index-api-openapi.yml
- filename: zincsearch-permission-api-openapi.yml
  format: yaml
  label: ZincSearch Permission API
  slug: zincsearch-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-permission-api-openapi.yml
- filename: zincsearch-role-api-openapi.yml
  format: yaml
  label: ZincSearch Role API
  slug: zincsearch-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-role-api-openapi.yml
- filename: zincsearch-search-api-openapi.yml
  format: yaml
  label: ZincSearch Search API
  slug: zincsearch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-search-api-openapi.yml
- filename: zincsearch-user-api-openapi.yml
  format: yaml
  label: ZincSearch User API
  slug: zincsearch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-user-api-openapi.yml
- filename: zincsearch-version-api-openapi.yml
  format: yaml
  label: ZincSearch Version API
  slug: zincsearch-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zincsearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZincSearch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZincSearch
provider_slug: zincsearch
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/zincsearch-openapi.yml
  type: http
slug: zincsearch-authentication
source_filename: zincsearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/zincsearch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/zincsearch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/authentication/zincsearch-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Search
- Full-Text Search
- Open Source
- Self-Hosted
- Elasticsearch Compatible
---
