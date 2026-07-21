---
api_key_in: []
api_specs:
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Product Reference Data API
  slug: unity-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Accounts & Balances API
  slug: unity-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Transactions API
  slug: unity-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Direct Debits & Scheduled Payments API
  slug: unity-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Payees API
  slug: unity-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Unity Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unity Bank secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unity Bank
provider_slug: unity-bank
scheme_count: 0
schemes: []
slug: unity-bank-authentication
source_filename: unity-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.unitybank.com.au/about-us/corporate-information/public-apis/\ndocs: https://www.unitybank.com.au/about-us/corporate-information/public-apis/\nnotes: >-\n  Documented (not merely spec-derived): Unity Bank's Public APIs page states the\n  Product API \"is public and does not require any authentication by consumers,\"\n  confirmed live with HTTP 200 responses to unauthenticated GETs (review.yml).\n  The harvested shared DSB spec declares no securitySchemes for the Product\n  Reference Data operations. Broader consumer data sharing follows the CDR\n  Accredited Data Recipient model.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nsurfaces:\n- name: product-reference-data\n  auth: none\n  public: true\n  detail: Unauthenticated public PRD; GET /banking/products and GET /banking/products/{productId}.\n  evidence: review.yml liveProbe (HTTP 200 without credentials); Public APIs page statement.\n- name:\
  \ consumer-data-sharing\n  auth: oauth2-oidc-fapi\n  public: false\n  scope: out-of-scope-of-public-prd\n  detail: >-\n    CDR Accredited Data Recipient (ADR) flows use the OIDC/FAPI 2.0 profile\n    (dynamic client registration, PAR, mTLS/private_key_jwt). Not part of the\n    public PRD surface and not independently exercised in this review.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/authentication/unity-bank-authentication.yml
summary_line: none · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
