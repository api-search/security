---
api_key_in:
- header
- query
api_specs:
- filename: ucd-cb-api-openapi.yml
  format: yaml
  label: University College Dublin CBÉ API
  slug: ucd-cb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-cb-api-openapi.yml
- filename: ucd-cb-d-api-openapi.yml
  format: yaml
  label: University College Dublin CBÉD API
  slug: ucd-cb-d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-cb-d-api-openapi.yml
- filename: ucd-cb-g-api-openapi.yml
  format: yaml
  label: University College Dublin CBÉG API
  slug: ucd-cb-g-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-cb-g-api-openapi.yml
- filename: ucd-cb-s-api-openapi.yml
  format: yaml
  label: University College Dublin CBÉS API
  slug: ucd-cb-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-cb-s-api-openapi.yml
- filename: ucd-metadata-api-openapi.yml
  format: yaml
  label: University College Dublin Metadata API
  slug: ucd-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-metadata-api-openapi.yml
- filename: ucd-reference-api-openapi.yml
  format: yaml
  label: University College Dublin Reference API
  slug: ucd-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-reference-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ucd Authentication
name_suffix: Authentication
oauth_flows: []
overview: University College Dublin secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University College Dublin
provider_slug: ucd
scheme_count: 3
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ucd-duchas.yaml
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/ucd-duchas.yaml
  type: apiKey
- description: Username is the API key; password is empty.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/ucd-duchas.yaml
  type: http
slug: ucd-authentication
source_filename: ucd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ucd-duchas.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ucd-duchas.yaml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/ucd-duchas.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Username is the API key; password is empty.\n  sources:\n  - openapi/ucd-duchas.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/authentication/ucd-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Education
- Higher Education
- University
- Ireland
- Library
- Digital Library
- IIIF
- Open Access
- Cultural Heritage
---
