---
api_key_in:
- query
api_specs:
- filename: serpapi-openapi.yml
  format: yaml
  label: SerpApi Bing API
  slug: serpapi-bing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serpapi/refs/heads/main/openapi/serpapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Serpapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SerpApi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SerpApi
provider_slug: serpapi
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/serpapi-openapi.yml
  type: apiKey
slug: serpapi-authentication
source_filename: serpapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/serpapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/serpapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpapi/refs/heads/main/authentication/serpapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bing
- Google
- Search
- Search Engines
---
