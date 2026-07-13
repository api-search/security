---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-search-openapi.yml
  format: yaml
  label: Azure AI Search REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-search/refs/heads/main/openapi/microsoft-azure-search-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure AI Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure AI Search
provider_slug: microsoft-azure-search
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/microsoft-azure-search-openapi.yml
  type: apiKey
slug: microsoft-azure-search-authentication
source_filename: microsoft-azure-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/microsoft-azure-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-search/refs/heads/main/authentication/microsoft-azure-search-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Search
- Cognitive Search
- Hybrid Search
- Search
- Semantic Search
- Vector Search
---
