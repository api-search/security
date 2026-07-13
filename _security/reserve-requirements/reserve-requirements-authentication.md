---
api_key_in:
- query
api_specs:
- filename: fred-openapi.yml
  format: yaml
  label: FRED API - Reserve Data
  slug: fred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reserve-requirements/refs/heads/main/openapi/fred-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reserve Requirements Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reserve Requirements secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reserve Requirements
provider_slug: reserve-requirements
scheme_count: 1
schemes:
- description: FRED API key obtained from api.stlouisfed.org/api/key.html
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/fred-openapi.yml
  type: apiKey
slug: reserve-requirements-authentication
source_filename: reserve-requirements-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fred-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: FRED API key obtained from api.stlouisfed.org/api/key.html\n  sources:\n  - openapi/fred-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reserve-requirements/refs/heads/main/authentication/reserve-requirements-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Reserve Requirements
- Federal Reserve
- Banking Regulation
- Monetary Policy
- Regulation D
- Finance
---
