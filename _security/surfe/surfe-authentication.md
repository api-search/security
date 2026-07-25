---
api_key_in: []
api_specs:
- filename: surfe-account-api-openapi.yml
  format: yaml
  label: Surfe Account API
  slug: surfe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-account-api-openapi.yml
- filename: surfe-companies-api-openapi.yml
  format: yaml
  label: Surfe Companies API
  slug: surfe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-companies-api-openapi.yml
- filename: surfe-people-api-openapi.yml
  format: yaml
  label: Surfe People API
  slug: surfe-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-people-api-openapi.yml
- filename: surfe-recommendations-api-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-recommendations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Surfe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surfe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Surfe
provider_slug: surfe
scheme_count: 1
schemes:
- description: 'Surfe API key issued from the Surfe dashboard, sent as `Authorization: Bearer {api-key}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/surfe-openapi.yml
  type: http
slug: surfe-authentication
source_filename: surfe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/surfe-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Surfe API key issued from the Surfe dashboard, sent as `Authorization: Bearer\n    {api-key}`.'\n  sources:\n  - openapi/surfe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/authentication/surfe-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B Data
- Contact Data
- Sales Intelligence
- Enrichment
- Lead Generation
- CRM
- Prospecting
---
