---
api_key_in:
- header
api_specs:
- filename: 6sense-company-identification-api-openapi.yml
  format: yaml
  label: 6sense Company Identification API
  slug: 6sense-company-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-identification-api-openapi.yml
- filename: 6sense-company-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Company Firmographics API
  slug: 6sense-company-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-firmographics-api-openapi.yml
- filename: 6sense-lead-scoring-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring API
  slug: 6sense-lead-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-api-openapi.yml
- filename: 6sense-lead-scoring-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring And Firmographics API
  slug: 6sense-lead-scoring-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-firmographics-api-openapi.yml
- filename: 6sense-people-enrichment-api-openapi.yml
  format: yaml
  label: 6sense People Enrichment API
  slug: 6sense-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-enrichment-api-openapi.yml
- filename: 6sense-people-search-api-openapi.yml
  format: yaml
  label: 6sense People Search API
  slug: 6sense-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 6Sense Authentication
name_suffix: Authentication
oauth_flows: []
overview: 6sense secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 6sense
provider_slug: 6sense
scheme_count: 1
schemes:
- description: 'Token-based auth. Format: `Token <api_token>`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/6sense-company-firmographics-api-openapi.yml
  - openapi/6sense-company-identification-api-openapi.yml
  - openapi/6sense-lead-scoring-api-openapi.yml
  - openapi/6sense-lead-scoring-firmographics-api-openapi.yml
  - openapi/6sense-people-enrichment-api-openapi.yml
  - openapi/6sense-people-search-api-openapi.yml
  type: apiKey
slug: 6sense-authentication
source_filename: 6sense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/6sense-company-firmographics-api-openapi.yml, openapi/6sense-company-identification-api-openapi.yml,\n  openapi/6sense-lead-scoring-api-openapi.yml, openapi/6sense-lead-scoring-firmographics-api-openapi.yml,\n  openapi/6sense-people-enrichment-api-openapi.yml, openapi/6sense-people-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based auth. Format: `Token <api_token>`.'\n  sources:\n  - openapi/6sense-company-firmographics-api-openapi.yml\n  - openapi/6sense-company-identification-api-openapi.yml\n  - openapi/6sense-lead-scoring-api-openapi.yml\n  - openapi/6sense-lead-scoring-firmographics-api-openapi.yml\n  - openapi/6sense-people-enrichment-api-openapi.yml\n  - openapi/6sense-people-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/authentication/6sense-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- AI
- Marketing Technology
---
