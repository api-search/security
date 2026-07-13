---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: TextGears API
  slug: textgears-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Textgears Authentication
name_suffix: Authentication
oauth_flows: []
overview: TextGears secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TextGears
provider_slug: textgears
scheme_count: 2
schemes:
- description: API key passed as a query parameter
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: API key passed as HTTP Basic Authorization header value
  name: apiKeyHeader
  scheme: basic
  sources:
  - openapi/openapi.yml
  type: http
slug: textgears-authentication
source_filename: textgears-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as a query parameter\n  sources:\n  - openapi/openapi.yml\n- name: apiKeyHeader\n  type: http\n  scheme: basic\n  description: API key passed as HTTP Basic Authorization header value\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/authentication/textgears-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Grammar
- Spelling
- Text Analysis
- Readability
- Natural Language Processing
- NLP
- Text Summarization
- Language Detection
---
