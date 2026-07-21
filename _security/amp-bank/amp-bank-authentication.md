---
api_key_in: []
api_specs:
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Product Reference Data API
  slug: amp-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank GO CDR Product Reference Data API
  slug: amp-bank-go-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Accounts & Balances API
  slug: amp-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Transactions API
  slug: amp-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Direct Debits & Scheduled Payments API
  slug: amp-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Payees API
  slug: amp-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
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
