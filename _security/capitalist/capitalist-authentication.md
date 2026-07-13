---
api_key_in:
- query
api_specs:
- filename: capitalist-openapi.yml
  format: yaml
  label: Capitalist API
  slug: capitalist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Capitalist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capitalist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capitalist
provider_slug: capitalist
scheme_count: 1
schemes:
- description: 'Capitalist authenticates via `login` and `password` form fields

    (the API also supports certificate-signed requests for elevated

    operations). Modeled as an apiKey here because OpenAPI does not

    natively express the form-credentials pattern.'
  in: query
  name: basicCreds
  parameter: login
  sources:
  - openapi/capitalist-openapi.yml
  type: apiKey
slug: capitalist-authentication
source_filename: capitalist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/capitalist-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: basicCreds\n  type: apiKey\n  in: query\n  parameter: login\n  description: |-\n    Capitalist authenticates via `login` and `password` form fields\n    (the API also supports certificate-signed requests for elevated\n    operations). Modeled as an apiKey here because OpenAPI does not\n    natively express the form-credentials pattern.\n  sources:\n  - openapi/capitalist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/authentication/capitalist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bulk Payouts
- Cryptocurrency
- Finance
- Mass Payments
- Payment Platform
- Payments
- Payouts
- Remittance
---
