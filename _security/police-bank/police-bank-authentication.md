---
api_key_in: []
api_specs:
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Product Reference Data API
  slug: police-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Accounts & Balances API
  slug: police-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Transactions API
  slug: police-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Direct Debits & Scheduled Payments API
  slug: police-bank-cds-banking-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Payees API
  slug: police-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Police Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Police Bank declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Police Bank
provider_slug: police-bank
scheme_count: 0
schemes: []
slug: police-bank-authentication
source_filename: police-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/police-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n# Police Bank publicly exposes only the unauthenticated Product Reference Data\n# (PRD) surface of the CDR Banking API. The PRD endpoints (/banking/products,\n# /banking/products/{productId}) require NO authentication - they are open,\n# machine-readable product data as mandated for every Australian ADI under the\n# Consumer Data Right. The OpenAPI declares no securitySchemes for these ops.\nsummary:\n  types: []\n  public_unauthenticated: true\n  api_key_in: []\n  oauth2_flows: []\nprd_surface:\n  authenticated: false\n  note: >-\n    No API key, token, or client credential is required to call the Product\n    Reference Data endpoints. A mandatory x-v request header selects the API\n    version but is not an auth credential.\nconsumer_data_sharing:\n  # The broader (authenticated) CDR data-sharing\
  \ flows are governed by the CDS\n  # security profile, not by a Police Bank-proprietary scheme. Police Bank\n  # participates as a data holder; members authenticate via the CDR consent\n  # flow with ACCC-accredited data recipients. These flows are NOT exposed on\n  # Police Bank's public surface.\n  standard: Consumer Data Standards security profile (FAPI 1.0 Advanced)\n  mechanisms: [OAuth2 authorization code + PKCE, OpenID Connect, PAR, MTLS-bound tokens]\n  applies_to: authenticated banking data sharing (accounts, transactions, etc.)\n  exposed_publicly: false\n  scopes: scopes/police-bank-scopes.yml  # 5 CDR banking scopes carried as x-scopes in the spec\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/authentication/police-bank-authentication.yml
summary_line: 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
---
