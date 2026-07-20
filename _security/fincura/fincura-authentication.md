---
api_key_in: []
api_specs:
- filename: fincura-openapi-original.yml
  format: yaml
  label: Automated Spreading and Analysis API
  slug: automated-spreading-and-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincura/refs/heads/main/openapi/fincura-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fincura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fincura secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fincura
provider_slug: fincura
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: API_Key
  scheme: bearer
  sources:
  - openapi/fincura-openapi-original.yml
  type: http
slug: fincura-authentication
source_filename: fincura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fincura-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: API_Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fincura-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincura/refs/heads/main/authentication/fincura-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Services
- Lending
- Credit Analysis
- Financial Spreading
- Banking
- Fintech
- Underwriting
- Company
---
