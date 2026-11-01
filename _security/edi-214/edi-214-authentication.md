---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: edi-214-claim-acknowledgments-api-openapi.yml
  format: yaml
  label: Edi 214 Claim acknowledgments API
  slug: edi-214-claim-acknowledgments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-claim-acknowledgments-api-openapi.yml
- filename: edi-214-claim-submission-api-openapi.yml
  format: yaml
  label: Edi 214 Claim submission API
  slug: edi-214-claim-submission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-claim-submission-api-openapi.yml
- filename: edi-214-coordination-of-benefits-api-openapi.yml
  format: yaml
  label: Edi 214 Coordination of benefits API
  slug: edi-214-coordination-of-benefits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-coordination-of-benefits-api-openapi.yml
- filename: edi-214-insurance-discovery-api-openapi.yml
  format: yaml
  label: Edi 214 Insurance discovery API
  slug: edi-214-insurance-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-insurance-discovery-api-openapi.yml
- filename: edi-214-payers-api-openapi.yml
  format: yaml
  label: Edi 214 Payers API
  slug: edi-214-payers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-payers-api-openapi.yml
- filename: edi-214-real-time-claim-status-api-openapi.yml
  format: yaml
  label: Edi 214 Real-time claim status API
  slug: edi-214-real-time-claim-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-real-time-claim-status-api-openapi.yml
- filename: edi-214-real-time-eligibility-check-api-openapi.yml
  format: yaml
  label: Edi 214 Real-time eligibility check API
  slug: edi-214-real-time-eligibility-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-real-time-eligibility-check-api-openapi.yml
- filename: edi-214-remittances-api-openapi.yml
  format: yaml
  label: Edi 214 Remittances API
  slug: edi-214-remittances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-remittances-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Edi 214 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edi 214 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edi 214
provider_slug: edi-214
scheme_count: 1
schemes:
- description: API key in format "Key {your_api_key}" for Stedi platform access
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/stedi-edi214-openapi.yml
  type: apiKey
slug: edi-214-authentication
source_filename: edi-214-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stedi-edi214-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key in format \"Key {your_api_key}\" for Stedi platform access\n  sources:\n  - openapi/stedi-edi214-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/edi-214/authentication/edi-214-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EDI
- Logistics
- Transaction
---
