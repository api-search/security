---
api_key_in:
- header
- query
api_specs:
- filename: news-api-openapi.yml
  format: yaml
  label: News API
  slug: news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/openapi/news-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: News Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: News API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: News API
provider_slug: news-api
scheme_count: 2
schemes:
- in: query
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/news-api-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/news-api-openapi.yml
  type: apiKey
slug: news-api-authentication
source_filename: news-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/news-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/news-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/news-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/authentication/news-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Articles
- Headlines
- Search
---
