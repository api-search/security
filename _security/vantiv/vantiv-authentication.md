---
api_key_in: []
api_specs:
- filename: vantiv-authorizations-api-openapi.yml
  format: yaml
  label: Vantiv Authorizations API
  slug: vantiv-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-authorizations-api-openapi.yml
- filename: vantiv-captures-api-openapi.yml
  format: yaml
  label: Vantiv Captures API
  slug: vantiv-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-captures-api-openapi.yml
- filename: vantiv-chargebacks-api-openapi.yml
  format: yaml
  label: Vantiv Chargebacks API
  slug: vantiv-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-chargebacks-api-openapi.yml
- filename: vantiv-credits-api-openapi.yml
  format: yaml
  label: Vantiv Credits API
  slug: vantiv-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-credits-api-openapi.yml
- filename: vantiv-documents-api-openapi.yml
  format: yaml
  label: Vantiv Documents API
  slug: vantiv-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-documents-api-openapi.yml
- filename: vantiv-echeck-api-openapi.yml
  format: yaml
  label: Vantiv eCheck API
  slug: vantiv-echeck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-echeck-api-openapi.yml
- filename: vantiv-recurring-api-openapi.yml
  format: yaml
  label: Vantiv Recurring API
  slug: vantiv-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-recurring-api-openapi.yml
- filename: vantiv-sales-api-openapi.yml
  format: yaml
  label: Vantiv Sales API
  slug: vantiv-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-sales-api-openapi.yml
- filename: vantiv-tokenization-api-openapi.yml
  format: yaml
  label: Vantiv Tokenization API
  slug: vantiv-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-tokenization-api-openapi.yml
- filename: vantiv-voids-api-openapi.yml
  format: yaml
  label: Vantiv Voids API
  slug: vantiv-voids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-voids-api-openapi.yml
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
