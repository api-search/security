---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marketparquet-api-v1-api-openapi.yml
  format: yaml
  label: MarketParquet API V1 API
  slug: marketparquet-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/openapi/marketparquet-api-v1-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Marketparquet Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketParquet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarketParquet
provider_slug: marketparquet
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marketparquet-openapi.json
  type: http
slug: marketparquet-authentication
source_filename: marketparquet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/marketparquet-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/marketparquet-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/authentication/marketparquet-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Data
- MarketData
- APIs
---
