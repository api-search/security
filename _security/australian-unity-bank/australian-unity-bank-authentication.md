---
api_key_in: []
api_specs:
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Product Reference Data API
  slug: australian-unity-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Accounts & Balances API
  slug: australian-unity-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Transactions API
  slug: australian-unity-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Direct Debits & Scheduled Payments API
  slug: australian-unity-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Payees API
  slug: australian-unity-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Australian Unity Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- hybrid
overview: Australian Unity Bank secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and hybrid flow(s).
provider_name: Australian Unity Bank
provider_slug: australian-unity-bank
scheme_count: 3
schemes:
- authorizationServer: https://open-banking.australianunity.com.au (OIDC discovery geo/WAF-gated; HTTP 403 to non-AU probe 2026-07-21)
  features:
  - private_key_jwt client authentication
  - Pushed Authorization Requests (PAR)
  - PKCE
  - request objects signed (JARM/signed responses)
  - mutual TLS sender-constrained access tokens
  - CDR Register trust framework (ADR accreditation + SSA)
  name: CDR-Security-Profile
  profile: FAPI 1.0 Advanced
  scopes_ref: scopes/australian-unity-bank-scopes.yml
  type: openIdConnect
- description: Mutual TLS is required on token and resource endpoints; access tokens are sender-constrained (holder-of-key).
  name: mTLS
  type: mutualTLS
- description: Product Reference Data endpoints are public and require no credentials.
  name: PublicPRD
  operations:
  - listBankingProducts
  - getBankingProductDetail
  type: none
slug: australian-unity-bank-authentication
source_filename: australian-unity-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnotes: >-\n  The harvested CDS Banking OpenAPI (v1.36.0) declares no securitySchemes because\n  the CDR authorization model lives in the separate DSB InfoSec / Security Profile.\n  Australian Unity Bank, as a CDR data holder, implements that shared profile.\n  Product Reference Data (products) endpoints are public/unauthenticated; all\n  consumer-data endpoints require the full CDR security profile.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  public_endpoints: [listBankingProducts, getBankingProductDetail]\n  oauth2_flows: [authorizationCode, hybrid]\nschemes:\n  - name: CDR-Security-Profile\n    type: openIdConnect\n    profile: FAPI 1.0 Advanced\n    features:\n      - private_key_jwt client authentication\n      - Pushed Authorization Requests (PAR)\n\
  \      - PKCE\n      - request objects signed (JARM/signed responses)\n      - mutual TLS sender-constrained access tokens\n      - CDR Register trust framework (ADR accreditation + SSA)\n    authorizationServer: https://open-banking.australianunity.com.au (OIDC discovery geo/WAF-gated; HTTP 403 to non-AU probe 2026-07-21)\n    scopes_ref: scopes/australian-unity-bank-scopes.yml\n  - name: mTLS\n    type: mutualTLS\n    description: Mutual TLS is required on token and resource endpoints; access tokens are sender-constrained (holder-of-key).\n  - name: PublicPRD\n    type: none\n    description: Product Reference Data endpoints are public and require no credentials.\n    operations: [listBankingProducts, getBankingProductDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/authentication/australian-unity-bank-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Product Reference Data
---
