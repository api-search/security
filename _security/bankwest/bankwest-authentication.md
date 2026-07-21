---
api_key_in: []
api_specs:
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Product Reference Data API
  slug: bankwest-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Accounts & Balances API
  slug: bankwest-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Transactions API
  slug: bankwest-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Direct Debits & Scheduled Payments API
  slug: bankwest-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Payees API
  slug: bankwest-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bankwest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bankwest secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bankwest
provider_slug: bankwest
scheme_count: 2
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  detail: Product APIs are publicly available; no authentication is required. Only the mandatory x-v version header must be supplied. Confirmed live (HTTP 200).
  name: publicPRD
  type: none
- applies_to: []
  detail: Access to consumer (customer-authorised) CDR data beyond PRD is NOT publicly callable. It requires ACCC accreditation as an Accredited Data Recipient and customer consent, using OAuth 2.0 / OpenID Connect under the FAPI 2.0 security profile with Pushed Authorization Requests (PAR) as mandated by the Consumer Data Standards. Bankwest publishes no self-onboarding path for this channel.
  name: cdrConsumerAuthorisation
  publicly_callable: false
  type: openIdConnect
slug: bankwest-authentication
source_filename: bankwest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.bankwest.com.au/support/open-banking/developers\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  The harvested OpenAPI declares no securitySchemes because the Product Reference\n  Data (PRD) endpoints are public. This profile is authored from Bankwest's\n  developer page and the DSB Consumer Data Standards security profile.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  public_surface: none\n  consumer_surface: oauth2 + openIdConnect (FAPI 2.0)\nschemes:\n- name: publicPRD\n  type: none\n  applies_to: [listBankingProducts, getBankingProductDetail]\n  detail: >-\n    Product APIs are publicly available; no authentication is required. Only the\n    mandatory x-v version header must be supplied. Confirmed live (HTTP 200).\n- name: cdrConsumerAuthorisation\n  type: openIdConnect\n  applies_to: []\n  publicly_callable: false\n  detail: >-\n    Access to consumer (customer-authorised)\
  \ CDR data beyond PRD is NOT publicly\n    callable. It requires ACCC accreditation as an Accredited Data Recipient and\n    customer consent, using OAuth 2.0 / OpenID Connect under the FAPI 2.0 security\n    profile with Pushed Authorization Requests (PAR) as mandated by the Consumer\n    Data Standards. Bankwest publishes no self-onboarding path for this channel.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/authentication/bankwest-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Digital Bank
---
