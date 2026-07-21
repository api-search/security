---
api_key_in: []
api_specs:
- filename: westpac-cds-banking-openapi.yml
  format: yaml
  label: Westpac Banking Corporation CDR Product Reference Data API
  slug: westpac-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-cds-banking-openapi.yml
- filename: westpac-cds-banking-openapi.yml
  format: yaml
  label: Westpac Banking Corporation CDR Accounts & Balances API
  slug: westpac-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-cds-banking-openapi.yml
- filename: westpac-cds-banking-openapi.yml
  format: yaml
  label: Westpac Banking Corporation CDR Transactions API
  slug: westpac-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-cds-banking-openapi.yml
- filename: westpac-cds-banking-openapi.yml
  format: yaml
  label: Westpac Banking Corporation CDR Direct Debits & Scheduled Payments API
  slug: westpac-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-cds-banking-openapi.yml
- filename: westpac-cds-banking-openapi.yml
  format: yaml
  label: Westpac Banking Corporation CDR Payees API
  slug: westpac-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-cds-banking-openapi.yml
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
