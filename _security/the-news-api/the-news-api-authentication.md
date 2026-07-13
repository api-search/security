---
api_key_in:
- query
api_specs:
- filename: the-news-api-openapi.yml
  format: yaml
  label: The News API
  slug: the-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-news-api/refs/heads/main/openapi/the-news-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The News Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: The News API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The News API
provider_slug: the-news-api
scheme_count: 1
schemes:
- in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/the-news-api-openapi.yml
  type: apiKey
slug: the-news-api-authentication
source_filename: the-news-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-news-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  sources:\n  - openapi/the-news-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-news-api/refs/heads/main/authentication/the-news-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Articles
- Headlines
- News
- Media
- Search
- International
---
