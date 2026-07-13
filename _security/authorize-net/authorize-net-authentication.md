---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Authorize Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authorize.net secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Authorize.net
provider_slug: authorize-net
scheme_count: 1
schemes:
- description: 'Authorize.Net does not use HTTP authentication. Instead, every request

    must include a `merchantAuthentication` object in the JSON/XML body

    containing the merchant''s API Login ID (`name`) and `transactionKey`.

    This security scheme entry is a placeholder so OpenAPI tooling can model

    the requirement.'
  in: header
  name: merchantAuthentication
  parameter: X-Anet-Merchant-Auth
  sources:
  - openapi/authorize-net-openapi.yml
  type: apiKey
slug: authorize-net-authentication
source_filename: authorize-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authorize-net-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: merchantAuthentication\n  type: apiKey\n  in: header\n  parameter: X-Anet-Merchant-Auth\n  description: |-\n    Authorize.Net does not use HTTP authentication. Instead, every request\n    must include a `merchantAuthentication` object in the JSON/XML body\n    containing the merchant's API Login ID (`name`) and `transactionKey`.\n    This security scheme entry is a placeholder so OpenAPI tooling can model\n    the requirement.\n  sources:\n  - openapi/authorize-net-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authorize-net/refs/heads/main/authentication/authorize-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accept.js
- Credit Cards
- eChecks
- Fraud Detection
- Payment Gateway
- Payments
- Recurring Billing
- Transactions
---
