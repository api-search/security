---
api_key_in:
- header
api_specs:
- filename: typesense-search-api-openapi.yml
  format: yaml
  label: Typesense Search API
  slug: typesense-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-search-api-openapi.yml
- filename: typesense-vector-search-api-openapi.yml
  format: yaml
  label: Typesense Vector Search API
  slug: typesense-vector-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-vector-search-api-openapi.yml
- filename: typesense-conversational-search-api-openapi.yml
  format: yaml
  label: Typesense Conversational Search API
  slug: typesense-conversational-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-conversational-search-api-openapi.yml
- filename: typesense-analytics-api-openapi.yml
  format: yaml
  label: Typesense Analytics API
  slug: typesense-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-analytics-api-openapi.yml
- filename: typesense-cloud-management-api-openapi.yml
  format: yaml
  label: Typesense Cloud Management API
  slug: typesense-cloud-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-cloud-management-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Typesense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Typesense secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Typesense
provider_slug: typesense
scheme_count: 2
schemes:
- description: API key for authenticating requests to the Typesense server.
  in: header
  name: api_key_header
  parameter: X-TYPESENSE-API-KEY
  sources:
  - openapi/typesense-analytics-api-openapi.yml
  - openapi/typesense-conversational-search-api-openapi.yml
  - openapi/typesense-search-api-openapi.yml
  - openapi/typesense-vector-search-api-openapi.yml
  type: apiKey
- description: Cloud management API key for authenticating requests to the Typesense Cloud Management API.
  in: header
  name: cloudApiKey
  parameter: X-TYPESENSE-CLOUD-MANAGEMENT-API-KEY
  sources:
  - openapi/typesense-cloud-management-api-openapi.yml
  type: apiKey
slug: typesense-authentication
source_filename: typesense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/typesense-analytics-api-openapi.yml, openapi/typesense-cloud-management-api-openapi.yml,\n  openapi/typesense-conversational-search-api-openapi.yml, openapi/typesense-search-api-openapi.yml,\n  openapi/typesense-vector-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key_header\n  type: apiKey\n  in: header\n  parameter: X-TYPESENSE-API-KEY\n  description: API key for authenticating requests to the Typesense server.\n  sources:\n  - openapi/typesense-analytics-api-openapi.yml\n  - openapi/typesense-conversational-search-api-openapi.yml\n  - openapi/typesense-search-api-openapi.yml\n  - openapi/typesense-vector-search-api-openapi.yml\n- name: cloudApiKey\n  type: apiKey\n  in: header\n  parameter: X-TYPESENSE-CLOUD-MANAGEMENT-API-KEY\n  description: Cloud management API key for authenticating requests to the Typesense Cloud Management\n    API.\n  sources:\n  - openapi/typesense-cloud-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/authentication/typesense-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Full-Text Search
- Open Source
- Search Engine
- Typo Tolerance
- Vector Search
---
