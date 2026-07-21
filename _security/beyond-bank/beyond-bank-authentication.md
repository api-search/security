---
api_key_in: []
api_specs:
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Product Reference Data API
  slug: beyond-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Accounts & Balances API
  slug: beyond-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Transactions API
  slug: beyond-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: beyond-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Payees API
  slug: beyond-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Beyond Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beyond Bank Australia secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beyond Bank Australia
provider_slug: beyond-bank
scheme_count: 4
schemes:
- description: The Product Reference Data endpoints (listBankingProducts, getBankingProductDetail) are public and unauthenticated — no API key, no OAuth token. Only the CDS versioning header (x-v) is required. Confirmed live returning HTTP 200 with x-v 5.
  name: public-prd-none
  operations:
  - listBankingProducts
  - getBankingProductDetail
  sources:
  - openapi/beyond-bank-cds-banking-products-openapi.yml
  tier: public-prd
  type: none
- description: Consumer data sharing (accounts, balances, transactions, direct debits, scheduled payments, payees) requires accredited Data Recipient status and explicit consumer consent through the CDR authorization flow. Access is over the mutually authenticated (mTLS) FAPI channel, not the public PRD host.
  features:
  - Pushed Authorization Requests (PAR)
  - request object signing (private_key_jwt client authentication)
  - mTLS sender-constrained access tokens
  - OIDC hybrid / authorization-code flow with consumer consent
  - Accredited Data Recipient registration via the CDR Register
  name: cdr-oauth2-fapi
  profile: FAPI 1.0 Advanced (CDR security profile)
  scheme: authorizationCode
  scopes_ref: scopes/beyond-bank-scopes.yml
  sources:
  - openapi/beyond-bank-cds-banking-products-openapi.yml
  tier: consumer-data
  type: oauth2
- description: Identity layer for the CDR authorization — OpenID Connect discovery, ID tokens, and consent are provided by Beyond Bank's CDR identity server, advertised via the CDR Register and the holder's OIDC discovery document.
  name: cdr-oidc
  tier: consumer-data
  type: openIdConnect
- description: Mutual TLS is mandatory on the CDR data-sharing channel; access tokens are bound to the client's mTLS certificate (sender-constrained) per FAPI. The public PRD host does not require client certificates.
  name: cdr-mtls
  tier: consumer-data
  type: mutualTLS
slug: beyond-bank-authentication
source_filename: beyond-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.beyondbank.com.au/open-banking/beyond-bank-product-apis/\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnotes: >-\n  Authentication profile for Beyond Bank Australia's CDR Banking surface. The harvested\n  DSB Consumer Data Standards contract declares no formal OpenAPI securitySchemes, so this\n  profile is documented from Beyond Bank's public open-banking pages and the published DSB\n  Consumer Data Standards security profile rather than mechanically derived. There are two\n  distinct tiers: an OPEN, unauthenticated Product Reference Data (PRD) surface, and a\n  consumer-authorised data-sharing surface secured by the CDR OAuth2/OIDC FAPI model.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  tiers: [public-prd, consumer-data]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: public-prd-none\n    tier: public-prd\n    type: none\n    description: >-\n\
  \      The Product Reference Data endpoints (listBankingProducts, getBankingProductDetail)\n      are public and unauthenticated — no API key, no OAuth token. Only the CDS versioning\n      header (x-v) is required. Confirmed live returning HTTP 200 with x-v 5.\n    operations: [listBankingProducts, getBankingProductDetail]\n    sources: [openapi/beyond-bank-cds-banking-products-openapi.yml]\n  - name: cdr-oauth2-fapi\n    tier: consumer-data\n    type: oauth2\n    scheme: authorizationCode\n    profile: FAPI 1.0 Advanced (CDR security profile)\n    features:\n      - Pushed Authorization Requests (PAR)\n      - request object signing (private_key_jwt client authentication)\n      - mTLS sender-constrained access tokens\n      - OIDC hybrid / authorization-code flow with consumer consent\n      - Accredited Data Recipient registration via the CDR Register\n    scopes_ref: scopes/beyond-bank-scopes.yml\n    description: >-\n      Consumer data sharing (accounts, balances, transactions,\
  \ direct debits, scheduled\n      payments, payees) requires accredited Data Recipient status and explicit consumer\n      consent through the CDR authorization flow. Access is over the mutually authenticated\n      (mTLS) FAPI channel, not the public PRD host.\n    sources: [openapi/beyond-bank-cds-banking-products-openapi.yml]\n  - name: cdr-oidc\n    tier: consumer-data\n    type: openIdConnect\n    description: >-\n      Identity layer for the CDR authorization — OpenID Connect discovery, ID tokens, and\n      consent are provided by Beyond Bank's CDR identity server, advertised via the CDR\n      Register and the holder's OIDC discovery document.\n  - name: cdr-mtls\n    tier: consumer-data\n    type: mutualTLS\n    description: >-\n      Mutual TLS is mandatory on the CDR data-sharing channel; access tokens are bound to\n      the client's mTLS certificate (sender-constrained) per FAPI. The public PRD host does\n      not require client certificates.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/authentication/beyond-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
---
