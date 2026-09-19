---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hiring-index-insights-api-openapi.yml
  format: yaml
  label: Hiring Index Insights API
  slug: hiring-index-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-insights-api-openapi.yml
- filename: hiring-index-job-api-openapi.yml
  format: yaml
  label: Hiring Index Job API
  slug: hiring-index-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-job-api-openapi.yml
- filename: hiring-index-search-api-openapi.yml
  format: yaml
  label: Hiring Index Search API
  slug: hiring-index-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hiring Index Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hiring Index secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hiring Index
provider_slug: hiring-index
scheme_count: 1
schemes:
- in: header
  name: rapidApiKey
  parameter: x-rapidapi-key
  sources:
  - openapi/hiring-index-openapi.yaml
  type: apiKey
slug: hiring-index-authentication
source_filename: hiring-index-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: derived\nsource: openapi/hiring-index-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rapidApiKey\n  type: apiKey\n  in: header\n  parameter: x-rapidapi-key\n  sources:\n  - openapi/hiring-index-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/authentication/hiring-index-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Job
- Hiring Data
- Labor Market
- Human Resources
- Recruiting
- Job Postings
- Market Intelligence
- Alternative Data
---
