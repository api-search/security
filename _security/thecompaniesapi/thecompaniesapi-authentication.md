---
api_key_in: []
api_specs:
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Search API
  slug: thecompaniesapi-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Enrichment API
  slug: thecompaniesapi-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Analytics API
  slug: thecompaniesapi-company-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Industries API
  slug: thecompaniesapi-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Technologies API
  slug: thecompaniesapi-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Locations API
  slug: thecompaniesapi-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Lists API
  slug: thecompaniesapi-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Actions API
  slug: thecompaniesapi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Job Titles Enrichment API
  slug: thecompaniesapi-job-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thecompaniesapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Companies API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Companies API
provider_slug: thecompaniesapi
scheme_count: 1
schemes:
- description: 'API token passed in the Authorization header. Create and manage tokens on your API tokens page in the account settings. New accounts receive 500 free credits (no credit card required) to start. Modeled note: the OpenAPI declares an apiKey scheme on the Authorization header; confirm whether a "Bearer " prefix is required against the live docs.'
  headerName: Authorization
  in: header
  name: apiKey
  sources:
  - openapi/thecompaniesapi-openapi.yml
  - https://www.thecompaniesapi.com/api
  type: apiKey
slug: thecompaniesapi-authentication
source_filename: thecompaniesapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thecompaniesapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  headerName: Authorization\n  description: 'API token passed in the Authorization header. Create and manage\n    tokens on your API tokens page in the account settings. New accounts receive\n    500 free credits (no credit card required) to start. Modeled note: the OpenAPI\n    declares an apiKey scheme on the Authorization header; confirm whether a\n    \"Bearer \" prefix is required against the live docs.'\n  sources:\n  - openapi/thecompaniesapi-openapi.yml\n  - https://www.thecompaniesapi.com/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/authentication/thecompaniesapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company Data
- Data Enrichment
- Firmographics
- Web Intelligence
- B2B Data
- Reference Data
- Company Search
---
