---
api_key_in: []
api_specs:
- filename: racq-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Balances API
  slug: racq-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-balances-api-openapi.yml
- filename: racq-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Direct Debits API
  slug: racq-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-direct-debits-api-openapi.yml
- filename: racq-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Scheduled Payments API
  slug: racq-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: racq-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Account Transactions API
  slug: racq-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-account-transactions-api-openapi.yml
- filename: racq-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Accounts API
  slug: racq-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-accounts-api-openapi.yml
- filename: racq-bank-banking-payees-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Payees API
  slug: racq-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-payees-api-openapi.yml
- filename: racq-bank-banking-products-api-openapi.yml
  format: yaml
  label: RACQ Bank Banking Products API
  slug: racq-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/openapi/racq-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Racq Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RACQ Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RACQ Bank
provider_slug: racq-bank
scheme_count: 0
schemes: []
slug: racq-bank-authentication
source_filename: racq-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.racq.com.au/banking/open-banking/api-access\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    RACQ Bank operates two distinct access channels under Australia's Consumer\n    Data Right (CDR). The Product Reference Data (PRD) endpoints are PUBLIC and\n    require NO authentication. The consumer data-sharing endpoints (accounts,\n    balances, transactions, direct debits, scheduled payments, payees) are only\n    reachable by an accredited data recipient (ADR) under the CDR security\n    profile and are not usable with a client-issued credential.\nchannels:\n  - name: Product Reference Data (PRD)\n    auth: none\n    public: true\n    operations: [listBankingProducts, getBankingProductDetail]\n    evidence: \"RACQ api-access page states: 'Authentication\
  \ is not required to access the Product APIs.'\"\n    base_url: https://cdrbank.racq.com.au/cds-au/v1\n  - name: Consumer Data Sharing\n    auth: [oauth2, openIdConnect, mutualTLS]\n    public: false\n    profile: CDR Security Profile (built on FAPI 1.0 Advanced + OIDC + PAR)\n    requires: Accreditation as a CDR Accredited Data Recipient (ADR) by the ACCC\n    mechanisms:\n      - OAuth 2.0 authorization_code flow with PKCE\n      - OpenID Connect (hybrid / authorization code)\n      - Pushed Authorization Requests (PAR, RFC 9126)\n      - Mutual TLS (MTLS) client authentication and sender-constrained tokens\n      - private_key_jwt client authentication\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/authentication/racq-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
- Mutual
---
