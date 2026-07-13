---
api_key_in:
- query
api_specs:
- filename: world-news-api-openapi.yml
  format: yaml
  label: World News API
  slug: world-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/world-news-api/refs/heads/main/openapi/world-news-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: World News Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: World News API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: World News API
provider_slug: world-news-api
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: api-key
  sources:
  - openapi/world-news-api-openapi.yml
  type: apiKey
slug: world-news-api-authentication
source_filename: world-news-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/world-news-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/world-news-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-news-api/refs/heads/main/authentication/world-news-api-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
