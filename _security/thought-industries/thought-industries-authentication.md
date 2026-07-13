---
api_key_in:
- header
- query
api_specs:
- filename: thought-industries-openapi.yml
  format: yaml
  label: Thought Industries REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thought-industries/refs/heads/main/openapi/thought-industries-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thought Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thought Industries secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thought Industries
provider_slug: thought-industries
scheme_count: 2
schemes:
- description: API key passed as X-API-Key request header.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/thought-industries-openapi.yml
  type: apiKey
- description: API key passed as apiKey query parameter.
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/thought-industries-openapi.yml
  type: apiKey
slug: thought-industries-authentication
source_filename: thought-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thought-industries-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed as X-API-Key request header.\n  sources:\n  - openapi/thought-industries-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key passed as apiKey query parameter.\n  sources:\n  - openapi/thought-industries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thought-industries/refs/heads/main/authentication/thought-industries-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Education
- Learning
- LMS
- LXP
- E-Learning
- Training
---
