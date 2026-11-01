---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nsgoods-org-health-api-openapi.yml
  format: yaml
  label: nsgoods-org Health API
  slug: nsgoods-org-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nsgoods-org/openapi/nsgoods-org-health-api-openapi.yml
- filename: nsgoods-org-payable-api-openapi.yml
  format: yaml
  label: nsgoods-org Payable API
  slug: nsgoods-org-payable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nsgoods-org/openapi/nsgoods-org-payable-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nsgoods Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: nsgoods-org secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: nsgoods-org
provider_slug: nsgoods-org
scheme_count: 1
schemes:
- description: x402 USDC payment on Base or Solana
  in: header
  name: x402Payment
  parameter: X-PAYMENT
  sources:
  - openapi/payable-nsgoods-org-openapi.json
  type: apiKey
slug: nsgoods-org-authentication
source_filename: nsgoods-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/payable-nsgoods-org-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 USDC payment on Base or Solana\n  sources:\n  - openapi/payable-nsgoods-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nsgoods-org/authentication/nsgoods-org-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Finance
- Blockchain
- Data
- Services
- Company
---
