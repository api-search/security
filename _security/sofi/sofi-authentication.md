---
api_key_in:
- header
api_specs:
- filename: sofi-affiliate-leads-api-openapi.yml
  format: yaml
  label: SoFi Affiliate Leads API
  slug: sofi-affiliate-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi/refs/heads/main/openapi/sofi-affiliate-leads-api-openapi.yml
- filename: sofi-partner-offers-api-openapi.yml
  format: yaml
  label: SoFi Partner Offers API
  slug: sofi-partner-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi/refs/heads/main/openapi/sofi-partner-offers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sofi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SoFi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SoFi
provider_slug: sofi
scheme_count: 1
schemes:
- description: Environment-specific accountId (QA or Production) issued by SoFi. Modeled here as an apiKey scheme; consult SoFi's affiliate documentation for exact placement.
  in: header
  name: accountIdKey
  parameter: accountId
  sources:
  - openapi/sofi-home-loan-affiliate-lead-api-openapi.yml
  - openapi/sofi-partner-offer-api-openapi.yml
  type: apiKey
slug: sofi-authentication
source_filename: sofi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/sofi-home-loan-affiliate-lead-api-openapi.yml, openapi/sofi-partner-offer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accountIdKey\n  type: apiKey\n  in: header\n  parameter: accountId\n  description: Environment-specific accountId (QA or Production) issued by SoFi. Modeled here\n    as an apiKey scheme; consult SoFi's affiliate documentation for exact placement.\n  sources:\n  - openapi/sofi-home-loan-affiliate-lead-api-openapi.yml\n  - openapi/sofi-partner-offer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi/refs/heads/main/authentication/sofi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Personal Finance
- Banking
- Lending
- Student Loans
- Mortgages
- Investing
- Credit Cards
- Fintech
- Open Banking
- Digital Banking
- Banking-as-a-Service
- Partner API
- Business Banking
- United States
---
