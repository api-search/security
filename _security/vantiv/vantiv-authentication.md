---
api_key_in: []
api_specs:
- filename: vantiv-cnp-openapi.yml
  format: yaml
  label: Vantiv CNP API
  slug: cnp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-cnp-openapi.yml
- filename: vantiv-express-openapi.yml
  format: yaml
  label: Vantiv Express API
  slug: express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-express-openapi.yml
- filename: vantiv-chargeback-openapi.yml
  format: yaml
  label: Vantiv Chargeback API
  slug: chargeback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-chargeback-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vantiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vantiv secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vantiv
provider_slug: vantiv
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/vantiv-chargeback-openapi.yml
  - openapi/vantiv-cnp-openapi.yml
  type: http
slug: vantiv-authentication
source_filename: vantiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vantiv-chargeback-openapi.yml, openapi/vantiv-cnp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/vantiv-chargeback-openapi.yml\n  - openapi/vantiv-cnp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/authentication/vantiv-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Processing
- eCommerce
- Finance
- FinTech
- Fortune 1000
---
