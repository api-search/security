---
api_key_in:
- query
api_specs:
- filename: valueserp-search-openapi.yml
  format: yaml
  label: ValueSERP Search API
  slug: valueserp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-search-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Valueserp Authentication
name_suffix: Authentication
oauth_flows: []
overview: ValueSERP secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ValueSERP
provider_slug: valueserp
scheme_count: 1
schemes:
- description: API key for authentication. Pass as the api_key query parameter. Use "demo" as the key for testing.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/valueserp-search-openapi.yml
  type: apiKey
slug: valueserp-authentication
source_filename: valueserp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/valueserp-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key for authentication. Pass as the api_key query parameter. Use \"demo\" as\n    the key for testing.\n  sources:\n  - openapi/valueserp-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/authentication/valueserp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SERP
- Search Engine Results
- Google Search
- Search API
- SEO
- Web Scraping
- Shopping Results
- News Search
- Image Search
- Local Search
- Places
- Data API
---
