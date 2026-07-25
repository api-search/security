---
api_key_in: []
api_specs:
- filename: amp-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Balances API
  slug: amp-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-balances-api-openapi.yml
- filename: amp-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Direct Debits API
  slug: amp-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-direct-debits-api-openapi.yml
- filename: amp-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Scheduled Payments API
  slug: amp-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: amp-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Transactions API
  slug: amp-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-transactions-api-openapi.yml
- filename: amp-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Accounts API
  slug: amp-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-accounts-api-openapi.yml
- filename: amp-bank-banking-payees-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Payees API
  slug: amp-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-payees-api-openapi.yml
- filename: amp-bank-banking-products-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Products API
  slug: amp-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-products-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Amp Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMP Bank declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AMP Bank
provider_slug: amp-bank
scheme_count: 0
schemes: []
slug: amp-bank-authentication
source_filename: amp-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/amp-bank-cds-banking-products-openapi.yml\nsummary:\n  types: []\n  authenticated: false\n  note: >-\n    The AMP Bank and AMP Bank GO surfaces captured in this repo are the CDR\n    Product Reference Data (PRD) endpoints (GET /banking/products and\n    /banking/products/{productId}). Per the DSB Consumer Data Standards, PRD is\n    a public, unauthenticated surface - the OpenAPI declares no securitySchemes\n    and requires no credential. The only mandatory request signalling is the\n    x-v (and optional x-min-v) CDS version header, not an auth header.\nschemes: []\ncontext:\n  regime: Consumer Data Right (CDR / Open Banking) - Australia\n  authenticated_surface: >-\n    The accredited consumer data sharing (non-PRD) surface, which is out of scope\n    of this published spec, is secured per the CDR Register/InfoSec profile:\n    FAPI 1.0 Advanced, OpenID Connect, OAuth 2.0, PAR, PKCE and mutual-TLS\n    sender-constrained\
  \ tokens. AMP does not expose that surface as public OpenAPI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/authentication/amp-bank-authentication.yml
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
