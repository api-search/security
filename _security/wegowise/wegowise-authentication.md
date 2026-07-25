---
api_key_in: []
api_specs:
- filename: wegowise-apartments-api-openapi.yml
  format: yaml
  label: WegoWise Apartments API
  slug: wegowise-apartments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-apartments-api-openapi.yml
- filename: wegowise-areas-api-openapi.yml
  format: yaml
  label: WegoWise Areas API
  slug: wegowise-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-areas-api-openapi.yml
- filename: wegowise-buildings-api-openapi.yml
  format: yaml
  label: WegoWise Buildings API
  slug: wegowise-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-buildings-api-openapi.yml
- filename: wegowise-developments-api-openapi.yml
  format: yaml
  label: WegoWise Developments API
  slug: wegowise-developments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-developments-api-openapi.yml
- filename: wegowise-meters-api-openapi.yml
  format: yaml
  label: WegoWise Meters API
  slug: wegowise-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-meters-api-openapi.yml
- filename: wegowise-usage-data-api-openapi.yml
  format: yaml
  label: WegoWise Usage Data API
  slug: wegowise-usage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-usage-data-api-openapi.yml
- filename: wegowise-utility-companies-api-openapi.yml
  format: yaml
  label: WegoWise Utility Companies API
  slug: wegowise-utility-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-utility-companies-api-openapi.yml
- filename: wegowise-utility-logins-api-openapi.yml
  format: yaml
  label: WegoWise Utility Logins API
  slug: wegowise-utility-logins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-utility-logins-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wegowise Authentication
name_suffix: Authentication
oauth_flows: []
overview: WegoWise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WegoWise
provider_slug: wegowise
scheme_count: 1
schemes:
- description: OAuth 1.0 authentication required for private endpoints
  name: oauth1
  scheme: oauth
  sources:
  - openapi/wegowise-openapi.yml
  type: http
slug: wegowise-authentication
source_filename: wegowise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wegowise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth1\n  type: http\n  scheme: oauth\n  description: OAuth 1.0 authentication required for private endpoints\n  sources:\n  - openapi/wegowise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/authentication/wegowise-authentication.yml
summary_line: http · 1 scheme
tags:
- Benchmarking
- Building Energy
- Energy Efficiency
- Multifamily
- Property Management
- Utility Data
---
