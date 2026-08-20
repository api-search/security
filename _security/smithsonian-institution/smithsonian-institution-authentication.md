---
api_key_in:
- query
api_specs:
- filename: smithsonian-institution-content-api-openapi.yml
  format: yaml
  label: Smithsonian Institution Content API
  slug: smithsonian-institution-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/openapi/smithsonian-institution-content-api-openapi.yml
- filename: smithsonian-institution-metrics-api-openapi.yml
  format: yaml
  label: Smithsonian Institution Metrics API
  slug: smithsonian-institution-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/openapi/smithsonian-institution-metrics-api-openapi.yml
- filename: smithsonian-institution-search-api-openapi.yml
  format: yaml
  label: Smithsonian Institution Search API
  slug: smithsonian-institution-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/openapi/smithsonian-institution-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smithsonian Institution Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smithsonian Institution secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smithsonian Institution
provider_slug: smithsonian-institution
scheme_count: 1
schemes:
- description: API key obtained by registering at api.data.gov
  in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/smithsonian-open-access-openapi.yml
  type: apiKey
slug: smithsonian-institution-authentication
source_filename: smithsonian-institution-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smithsonian-open-access-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key obtained by registering at api.data.gov\n  sources:\n  - openapi/smithsonian-open-access-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/authentication/smithsonian-institution-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Collection
- Cultural Heritage
- Museums
- Open Data
- Art
- Natural History
- Research
---
