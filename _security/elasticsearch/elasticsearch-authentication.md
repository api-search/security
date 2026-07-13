---
api_key_in:
- header
api_specs:
- filename: elasticsearch-specification
  format: yaml
  label: Elasticsearch REST API
  slug: elasticsearch-rest-api
  spec_type: OpenAPI
  url: https://github.com/elastic/elasticsearch-specification
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elasticsearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elasticsearch secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elasticsearch
provider_slug: elasticsearch
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elasticsearch-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elasticsearch-openapi.yml
  type: apiKey
slug: elasticsearch-authentication
source_filename: elasticsearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elasticsearch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elasticsearch-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/elasticsearch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/authentication/elasticsearch-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Database
- Full-Text Search
- NoSQL
- Search
---
