---
api_key_in:
- query
api_specs:
- filename: congress-gov-api-openapi.yml
  format: yaml
  label: Congress.gov API
  slug: congress-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-house-of-representatives/refs/heads/main/openapi/congress-gov-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us House Of Representatives Authentication
name_suffix: Authentication
oauth_flows: []
overview: US House of Representatives secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: US House of Representatives
provider_slug: us-house-of-representatives
scheme_count: 1
schemes:
- description: API key required for all requests. Register at https://api.congress.gov/sign-up to obtain a key.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/congress-gov-api-openapi.yml
  type: apiKey
slug: us-house-of-representatives-authentication
source_filename: us-house-of-representatives-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/congress-gov-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key required for all requests. Register at https://api.congress.gov/sign-up\n    to obtain a key.\n  sources:\n  - openapi/congress-gov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-house-of-representatives/refs/heads/main/authentication/us-house-of-representatives-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Legislation
- Congress
- Legislative Data
- Bills
- Members
- Committees
---
