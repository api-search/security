---
api_key_in: []
api_specs:
- filename: westpac-banking-account-balances-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Balances API
  slug: westpac-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-balances-api-openapi.yml
- filename: westpac-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Direct Debits API
  slug: westpac-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-direct-debits-api-openapi.yml
- filename: westpac-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Scheduled Payments API
  slug: westpac-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-scheduled-payments-api-openapi.yml
- filename: westpac-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Transactions API
  slug: westpac-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-transactions-api-openapi.yml
- filename: westpac-banking-accounts-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Accounts API
  slug: westpac-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-accounts-api-openapi.yml
- filename: westpac-banking-payees-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Payees API
  slug: westpac-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-payees-api-openapi.yml
- filename: westpac-banking-products-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Products API
  slug: westpac-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-products-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Westpac Authentication
name_suffix: Authentication
oauth_flows: []
overview: Westpac Banking Corporation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Westpac Banking Corporation
provider_slug: westpac
scheme_count: 0
schemes: []
slug: westpac-authentication
source_filename: westpac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/westpac-cds-banking-products-openapi.yml\ndocs: https://www.westpac.com.au/about-westpac/innovation/open-banking/product-api/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The Westpac CDR Product Reference Data OpenAPI declares NO securitySchemes and\n    applies NO security requirement to either operation. Westpac's own\n    documentation confirms \"no security or other headers are required to call this\n    API\" beyond the mandatory x-v version header. The public PRD surface is\n    unauthenticated by design under the Consumer Data Standards.\nschemes: []\npublic_access:\n  authenticated: false\n  detail: >-\n    listProducts and getProductDetail are open, unauthenticated GET endpoints.\nconsumer_data_sharing:\n  detail: >-\n    Access to consumer/account data beyond product reference data is NOT available\n    through this public API. It flows through the CDR's Accredited Data Recipient\n\
  \    (ADR) model, which uses an OAuth 2.0 / OpenID Connect, FAPI-hardened consent\n    flow operated through the CDR ecosystem (accreditation + the CDR Register),\n    not a Westpac-issued developer credential. That surface is out of scope for\n    this public PRD contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/authentication/westpac-authentication.yml
summary_line: 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
