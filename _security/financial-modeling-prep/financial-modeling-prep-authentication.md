---
api_key_in:
- query
api_specs:
- filename: financial-modeling-prep-openapi.yml
  format: yaml
  label: Financial Modeling Prep API
  slug: financial-modeling-prep
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Financial Modeling Prep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Financial Modeling Prep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Financial Modeling Prep
provider_slug: financial-modeling-prep
scheme_count: 1
schemes:
- in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/financial-modeling-prep-openapi.yml
  type: apiKey
slug: financial-modeling-prep-authentication
source_filename: financial-modeling-prep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/financial-modeling-prep-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/financial-modeling-prep-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/authentication/financial-modeling-prep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Data
- Market Data
- Stocks
- Quotes
- Fundamentals
- Financial Statements
- Historical
---
