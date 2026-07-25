---
api_key_in: []
api_specs:
- filename: surfe-b2b-account-api-openapi.yml
  format: yaml
  label: Surfe Account API
  slug: surfe-b2b-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-account-api-openapi.yml
- filename: surfe-b2b-companies-api-openapi.yml
  format: yaml
  label: Surfe Companies API
  slug: surfe-b2b-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-companies-api-openapi.yml
- filename: surfe-b2b-people-api-openapi.yml
  format: yaml
  label: Surfe People API
  slug: surfe-b2b-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-people-api-openapi.yml
- filename: surfe-b2b-recommendations-api-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-b2b-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-recommendations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Surfe B2B Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surfe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Surfe
provider_slug: surfe-b2b
scheme_count: 1
schemes:
- description: 'Surfe API key issued from the Surfe dashboard, sent as `Authorization: Bearer {api-key}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/surfe-b2b-openapi.yml
  type: http
slug: surfe-b2b-authentication
source_filename: surfe-b2b-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/surfe-b2b-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Surfe API key issued from the Surfe dashboard, sent as `Authorization: Bearer\n    {api-key}`.'\n  sources:\n  - openapi/surfe-b2b-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/authentication/surfe-b2b-authentication.yml
summary_line: http · 1 scheme
tags:
- Contact Discovery
- Data Enrichment
- B2B Data
- Sales Intelligence
- Lead Enrichment
- Web Intelligence
- Contact Data
- People Enrichment
- Company Enrichment
- Prospecting
---
