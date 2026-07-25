---
api_key_in:
- header
api_specs:
- filename: diamond-search-fullfeed-api-openapi.yml
  format: yaml
  label: Diamond Search Fullfeed API
  slug: diamond-search-fullfeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/diamond-search-fullfeed-api-openapi.yml
- filename: diamond-search-getreport3-api-openapi.yml
  format: yaml
  label: Diamond Search Getreport3 API
  slug: diamond-search-getreport3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/diamond-search-getreport3-api-openapi.yml
- filename: diamond-search-labgrownfullfile-api-openapi.yml
  format: yaml
  label: Diamond Search Labgrownfullfile API
  slug: diamond-search-labgrownfullfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/diamond-search-labgrownfullfile-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Diamond Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diamond Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diamond Search
provider_slug: diamond-search
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/idex-lab-grown-file-api-openapi.yml
  type: apiKey
slug: diamond-search-authentication
source_filename: diamond-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/idex-lab-grown-file-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/idex-lab-grown-file-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/authentication/diamond-search-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Diamonds
- Lab Grown
- Pricing
- Trading
---
