---
api_key_in:
- header
api_specs:
- filename: bjs-ncvs-api-openapi.yml
  format: yaml
  label: BJS NCVS API
  slug: ncvs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/openapi/bjs-ncvs-api-openapi.yml
- filename: bjs-nibrs-api-openapi.yml
  format: yaml
  label: BJS NIBRS National Estimates API
  slug: nibrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/openapi/bjs-nibrs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Data Analysis Tools Bureau Of Justice Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Justice Statistics Data Analysis Tools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bureau of Justice Statistics Data Analysis Tools
provider_slug: data-analysis-tools-bureau-of-justice-statistics
scheme_count: 1
schemes:
- description: Optional Socrata application token for higher rate limits.
  in: header
  name: appToken
  parameter: X-App-Token
  sources:
  - openapi/bjs-ncvs-api-openapi.yml
  - openapi/bjs-nibrs-api-openapi.yml
  type: apiKey
slug: data-analysis-tools-bureau-of-justice-statistics-authentication
source_filename: data-analysis-tools-bureau-of-justice-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bjs-ncvs-api-openapi.yml, openapi/bjs-nibrs-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: Optional Socrata application token for higher rate limits.\n  sources:\n  - openapi/bjs-ncvs-api-openapi.yml\n  - openapi/bjs-nibrs-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/authentication/data-analysis-tools-bureau-of-justice-statistics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crime Statistics
- Federal Government
- NCVS
- NIBRS
- Open Data
- SODA
- Statistics
- Victimization
---
