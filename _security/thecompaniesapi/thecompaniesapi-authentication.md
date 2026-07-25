---
api_key_in: []
api_specs:
- filename: thecompaniesapi-actions-api-openapi.yml
  format: yaml
  label: The Companies API actions API
  slug: thecompaniesapi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-actions-api-openapi.yml
- filename: thecompaniesapi-analytics-api-openapi.yml
  format: yaml
  label: The Companies API analytics API
  slug: thecompaniesapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-analytics-api-openapi.yml
- filename: thecompaniesapi-companies-api-openapi.yml
  format: yaml
  label: The Companies API companies API
  slug: thecompaniesapi-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-companies-api-openapi.yml
- filename: thecompaniesapi-industries-api-openapi.yml
  format: yaml
  label: The Companies API industries API
  slug: thecompaniesapi-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-industries-api-openapi.yml
- filename: thecompaniesapi-job-titles-api-openapi.yml
  format: yaml
  label: The Companies API job-titles API
  slug: thecompaniesapi-job-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-job-titles-api-openapi.yml
- filename: thecompaniesapi-lists-api-openapi.yml
  format: yaml
  label: The Companies API lists API
  slug: thecompaniesapi-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-lists-api-openapi.yml
- filename: thecompaniesapi-locations-api-openapi.yml
  format: yaml
  label: The Companies API locations API
  slug: thecompaniesapi-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-locations-api-openapi.yml
- filename: thecompaniesapi-prompts-api-openapi.yml
  format: yaml
  label: The Companies API prompts API
  slug: thecompaniesapi-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-prompts-api-openapi.yml
- filename: thecompaniesapi-teams-api-openapi.yml
  format: yaml
  label: The Companies API teams API
  slug: thecompaniesapi-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-teams-api-openapi.yml
- filename: thecompaniesapi-technologies-api-openapi.yml
  format: yaml
  label: The Companies API technologies API
  slug: thecompaniesapi-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-technologies-api-openapi.yml
- filename: thecompaniesapi-users-api-openapi.yml
  format: yaml
  label: The Companies API users API
  slug: thecompaniesapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-users-api-openapi.yml
- filename: thecompaniesapi-utilities-api-openapi.yml
  format: yaml
  label: The Companies API utilities API
  slug: thecompaniesapi-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-utilities-api-openapi.yml
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
