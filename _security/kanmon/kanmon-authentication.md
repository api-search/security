---
api_key_in:
- header
api_specs:
- filename: kanmon-bank-accounts-api-openapi.yml
  format: yaml
  label: Kanmon Bank Accounts API
  slug: kanmon-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-bank-accounts-api-openapi.yml
- filename: kanmon-businesses-api-openapi.yml
  format: yaml
  label: Kanmon Businesses API
  slug: kanmon-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-businesses-api-openapi.yml
- filename: kanmon-connect-tokens-api-openapi.yml
  format: yaml
  label: Kanmon Connect Tokens API
  slug: kanmon-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-connect-tokens-api-openapi.yml
- filename: kanmon-documents-api-openapi.yml
  format: yaml
  label: Kanmon Documents API
  slug: kanmon-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-documents-api-openapi.yml
- filename: kanmon-draw-requests-api-openapi.yml
  format: yaml
  label: Kanmon Draw Requests API
  slug: kanmon-draw-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-draw-requests-api-openapi.yml
- filename: kanmon-embedded-sessions-api-openapi.yml
  format: yaml
  label: Kanmon Embedded Sessions API
  slug: kanmon-embedded-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-embedded-sessions-api-openapi.yml
- filename: kanmon-integrated-mca-api-openapi.yml
  format: yaml
  label: Kanmon Integrated MCA API
  slug: kanmon-integrated-mca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-integrated-mca-api-openapi.yml
- filename: kanmon-invoices-api-openapi.yml
  format: yaml
  label: Kanmon Invoices API
  slug: kanmon-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-invoices-api-openapi.yml
- filename: kanmon-issued-products-api-openapi.yml
  format: yaml
  label: Kanmon Issued Products API
  slug: kanmon-issued-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-issued-products-api-openapi.yml
- filename: kanmon-offers-api-openapi.yml
  format: yaml
  label: Kanmon Offers API
  slug: kanmon-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-offers-api-openapi.yml
- filename: kanmon-payments-api-openapi.yml
  format: yaml
  label: Kanmon Payments API
  slug: kanmon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-payments-api-openapi.yml
- filename: kanmon-prequalifications-api-openapi.yml
  format: yaml
  label: Kanmon Prequalifications API
  slug: kanmon-prequalifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-prequalifications-api-openapi.yml
- filename: kanmon-sandbox-utilities-api-openapi.yml
  format: yaml
  label: Kanmon Sandbox Utilities API
  slug: kanmon-sandbox-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-sandbox-utilities-api-openapi.yml
- filename: kanmon-users-api-openapi.yml
  format: yaml
  label: Kanmon Users API
  slug: kanmon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kanmon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kanmon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kanmon
provider_slug: kanmon
scheme_count: 1
schemes:
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/kanmon-openapi-original.yml
  type: apiKey
slug: kanmon-authentication
source_filename: kanmon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kanmon-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/kanmon-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/authentication/kanmon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Embedded Finance
- Embedded Lending
- Lending
- Working Capital
- Invoice Financing
---
