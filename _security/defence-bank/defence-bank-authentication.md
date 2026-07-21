---
api_key_in: []
api_specs:
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Product Reference Data API
  slug: defence-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Accounts & Balances API
  slug: defence-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Transactions API
  slug: defence-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Direct Debits & Scheduled Payments API
  slug: defence-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Payees API
  slug: defence-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: The Consumer Data Standards banking spec published for Defence Bank declares no inline OpenAPI securitySchemes, because authentication in the CDR is split by endpoint class. This profile is captured from the CDS security profile and the provider's open banking documentation.
kind: authentication
layout: security
method: searched
name: Defence Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode-hybrid
overview: Defence Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode-hybrid flow(s).
provider_name: Defence Bank
provider_slug: defence-bank
scheme_count: 2
schemes:
- applies_to: consumer-data-sharing endpoints
  name: CDR-FAPI-OAuth2
  profile: FAPI (MTLS-bound tokens, OIDC hybrid, PAR)
  scheme: authorizationCode
  sources:
  - Consumer Data Standards security profile
  type: oauth2
- applies_to: consumer-data-sharing endpoints (token binding + holder-of-key)
  name: MTLS
  sources:
  - Consumer Data Standards security profile
  type: mutualTLS
slug: defence-bank-authentication
source_filename: defence-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/defence-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndescription: >-\n  The Consumer Data Standards banking spec published for Defence Bank declares no\n  inline OpenAPI securitySchemes, because authentication in the CDR is split by\n  endpoint class. This profile is captured from the CDS security profile and the\n  provider's open banking documentation.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode-hybrid]\ntiers:\n- tier: product-reference-data\n  auth: none\n  description: >-\n    The Product Reference Data (PRD) endpoints (/banking/products and\n    /banking/products/{productId}) are public and unauthenticated. Confirmed live:\n    GET https://product.defencebank.com.au/cds-au/v1/banking/products with header\n    x-v: 4 returns HTTP 200. No credentials, API key, or token\
  \ are required.\n  operations: [listBankingProducts, getBankingProductDetail]\n- tier: consumer-data-sharing\n  auth: cdr-fapi\n  description: >-\n    All account/transaction/balance/direct-debit/scheduled-payment/payee endpoints\n    require the CDR FAPI security profile: OAuth2 authorization-code (OIDC hybrid)\n    with the consumer's consent, mutual-TLS-bound access tokens, request-object\n    signing, and the x-fapi-interaction-id / x-fapi-auth-date headers. Only\n    Accredited Data Recipients (ADRs) registered on the CDR Register can obtain\n    tokens. Access is scoped by CDR authorization scopes (see scopes/).\n  scopes: [bank:accounts.basic:read, bank:accounts.detail:read, bank:transactions:read, bank:regular_payments:read, bank:payees:read]\nschemes:\n- name: CDR-FAPI-OAuth2\n  type: oauth2\n  scheme: authorizationCode\n  profile: FAPI (MTLS-bound tokens, OIDC hybrid, PAR)\n  applies_to: consumer-data-sharing endpoints\n  sources: [Consumer Data Standards security profile]\n\
  - name: MTLS\n  type: mutualTLS\n  applies_to: consumer-data-sharing endpoints (token binding + holder-of-key)\n  sources: [Consumer Data Standards security profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/authentication/defence-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 2 schemes
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
