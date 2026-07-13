---
api_key_in:
- query
api_specs:
- filename: index.htm
  format: yaml
  label: The Bureau of Economic Analysis API
  slug: the-bureau-of-economic-analysis
  spec_type: OpenAPI
  url: https://apps.bea.gov/API/docs/index.htm
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Bureau Of Economic Analysis Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Bureau of Economic Analysis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Bureau of Economic Analysis
provider_slug: the-bureau-of-economic-analysis
scheme_count: 1
schemes:
- description: BEA API key obtained by registering at https://apps.bea.gov/api/signup/
  in: query
  name: ApiKeyAuth
  parameter: UserID
  sources:
  - openapi/the-bureau-of-economic-analysis-openapi.yml
  type: apiKey
slug: the-bureau-of-economic-analysis-authentication
source_filename: the-bureau-of-economic-analysis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-bureau-of-economic-analysis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: UserID\n  description: BEA API key obtained by registering at https://apps.bea.gov/api/signup/\n  sources:\n  - openapi/the-bureau-of-economic-analysis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-bureau-of-economic-analysis/refs/heads/main/authentication/the-bureau-of-economic-analysis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Economics
- Federal Government
- GDP
- National Accounts
- Open Data
- Statistics
---
