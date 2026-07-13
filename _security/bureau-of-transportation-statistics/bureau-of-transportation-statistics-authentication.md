---
api_key_in:
- header
api_specs:
- filename: bureau-of-transportation-statistics-openapi.yml
  format: yaml
  label: BTS Open Data SODA API
  slug: bts-open-data-soda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/openapi/bureau-of-transportation-statistics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bureau Of Transportation Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Transportation Statistics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bureau of Transportation Statistics
provider_slug: bureau-of-transportation-statistics
scheme_count: 1
schemes:
- description: Socrata application token from data.bts.gov developer registration.
  in: header
  name: appToken
  parameter: X-App-Token
  sources:
  - openapi/bureau-of-transportation-statistics-openapi.yml
  type: apiKey
slug: bureau-of-transportation-statistics-authentication
source_filename: bureau-of-transportation-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bureau-of-transportation-statistics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: Socrata application token from data.bts.gov developer registration.\n  sources:\n  - openapi/bureau-of-transportation-statistics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/authentication/bureau-of-transportation-statistics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Statistics
- Transportation
- Aviation
- Freight
- Open Data
---
