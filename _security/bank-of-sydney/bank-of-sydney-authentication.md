---
api_key_in: []
api_specs:
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Product Reference Data API
  slug: bank-of-sydney-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Accounts & Balances API
  slug: bank-of-sydney-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Transactions API
  slug: bank-of-sydney-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Direct Debits & Scheduled Payments API
  slug: bank-of-sydney-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Payees API
  slug: bank-of-sydney-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bank Of Sydney Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bank of Sydney secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bank of Sydney
provider_slug: bank-of-sydney
scheme_count: 4
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  description: Public, unauthenticated Product Reference Data endpoints (listBankingProducts, getBankingProductDetail). No credential required; only the x-v version header.
  name: publicProductReferenceData
  sources:
  - openapi/bank-of-sydney-cds-banking-products-openapi.yml
  type: none
- description: CDR authorisation via OAuth2 authorization-code flow. Authorization/token endpoints are published on the data holder's CDR authorization server (OIDC discovery), not on the resource host. Tokens are FAPI sender-constrained.
  name: cdrOAuth2
  scheme: authorizationCode
  scopes:
  - bank:accounts.basic:read
  - bank:accounts.detail:read
  - bank:transactions:read
  - bank:payees:read
  - bank:regular_payments:read
  sources:
  - openapi/bank-of-sydney-cds-banking-products-openapi.yml
  type: oauth2
- description: OpenID Connect (CDR profile) for authenticating the consumer and issuing the ID token during the CDR consent/authorisation flow.
  name: cdrOIDC
  sources:
  - Consumer Data Standards CDR security profile
  type: openIdConnect
- description: Mutual-TLS (FAPI holder-of-key). Accredited Data Recipients present a client certificate; access tokens are bound to the presented certificate. The CDS spec servers[] advertise mtls.dh.example.com / tls.dh.example.com placeholder hosts for the MTLS and TLS variants.
  name: cdrMutualTLS
  sources:
  - Consumer Data Standards CDR security profile
  type: mutualTLS
slug: bank-of-sydney-authentication
source_filename: bank-of-sydney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  Consumer Data Standards (DSB) CDR security profile + Bank of Sydney Open Banking\n  page (https://www.banksyd.com.au/tools-support/open-banking/); the harvested CDS\n  banking spec expresses scopes via the x-scopes extension rather than an OpenAPI\n  securitySchemes block, so this profile is captured from the CDR regime it implements.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_surface: >-\n    Product Reference Data (Get Products / Get Product Detail) is public and\n    unauthenticated per the Consumer Data Standards - no API key or token required.\n  authenticated_surface: >-\n    All consumer account/transaction/payee/payment endpoints require CDR\n    authorisation: an Accredited Data Recipient (ADR) acting under active consumer\n    consent, using OAuth2 authorization-code + OpenID Connect hardened by the\n    FAPI-based CDR security profile, with mutual-TLS holder-of-key sender-constrained\n\
  \    tokens. No self-serve public developer credentials are issued outside the ADR\n    ecosystem.\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\nschemes:\n  - name: publicProductReferenceData\n    type: none\n    description: >-\n      Public, unauthenticated Product Reference Data endpoints (listBankingProducts,\n      getBankingProductDetail). No credential required; only the x-v version header.\n    applies_to: [listBankingProducts, getBankingProductDetail]\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - name: cdrOAuth2\n    type: oauth2\n    scheme: authorizationCode\n    description: >-\n      CDR authorisation via OAuth2 authorization-code flow. Authorization/token\n      endpoints are published on the data holder's CDR authorization server (OIDC\n      discovery), not on the resource host. Tokens are FAPI sender-constrained.\n    scopes:\n      - bank:accounts.basic:read\n      - bank:accounts.detail:read\n      - bank:transactions:read\n \
  \     - bank:payees:read\n      - bank:regular_payments:read\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - name: cdrOIDC\n    type: openIdConnect\n    description: >-\n      OpenID Connect (CDR profile) for authenticating the consumer and issuing the\n      ID token during the CDR consent/authorisation flow.\n    sources: [Consumer Data Standards CDR security profile]\n  - name: cdrMutualTLS\n    type: mutualTLS\n    description: >-\n      Mutual-TLS (FAPI holder-of-key). Accredited Data Recipients present a client\n      certificate; access tokens are bound to the presented certificate. The CDS\n      spec servers[] advertise mtls.dh.example.com / tls.dh.example.com placeholder\n      hosts for the MTLS and TLS variants.\n    sources: [Consumer Data Standards CDR security profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/authentication/bank-of-sydney-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
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
