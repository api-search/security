---
api_key_in: []
api_specs:
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Product Reference Data API
  slug: banksa-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Accounts & Balances API
  slug: banksa-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Transactions API
  slug: banksa-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Direct Debits & Scheduled Payments API
  slug: banksa-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Payees API
  slug: banksa-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Banksa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BankSA secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BankSA
provider_slug: banksa
scheme_count: 4
schemes:
- applies_to:
  - GET /banking/products
  - GET /banking/products/{productId}
  description: Product Reference Data (PRD) endpoints are mandated by the CDR to be public and unauthenticated. BankSA's live host returns HTTP 200 for these with no Authorization header and no client certificate. A valid x-v version header is still required (see conventions/banksa-conventions.yml).
  name: PublicProductReferenceData
  sources:
  - openapi/banksa-cds-banking-products-openapi.yml
  type: none
- description: 'All consumer-data endpoints in this spec (accounts, balances, transactions, direct debits, scheduled payments, payees) are only reachable by an accredited data recipient (ADR) acting on a consumer''s behalf. Authorization uses OAuth 2.0 authorization-code with the OpenID Connect hybrid flow under the FAPI 1.0 Advanced profile: Pushed Authorization Requests (PAR), PKCE, request objects (JAR), and confirmation of the consumer''s consent via the CDR authorization server. Tokens are bound with mTLS sender-constrained access tokens.'
  flows:
  - detail: scopes/banksa-scopes.yml
    flow: authorizationCode
    scopes: 9
  name: CDRConsumerDataSharing
  scheme: FAPI 1.0 Advanced authorization-code with PAR + PKCE
  sources:
  - openapi/banksa-cds-banking-products-openapi.yml
  type: oauth2
- description: The data-holder resource server is exposed on an mTLS endpoint (the OpenAPI server is described as "MTLS"). Accredited data recipients present a client certificate issued through the CDR Register PKI; access tokens are sender-constrained (bound to the client certificate) per FAPI.
  name: CDRmTLS
  sources:
  - openapi/banksa-cds-banking-products-openapi.yml
  type: mutualTLS
- description: Consumer authentication and consent are brokered through the data holder's OpenID Provider, discovered by ADRs via the CDR Register rather than a public /.well-known/openid-configuration on digital-api.banksa.com.au.
  name: CDROpenIDConnect
  sources:
  - openapi/banksa-cds-banking-products-openapi.yml
  type: openIdConnect
slug: banksa-authentication
source_filename: banksa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  and the CDR Register / InfoSec profile. The harvested OpenAPI\n  (openapi/banksa-cds-banking-products-openapi.yml) declares no inline\n  securitySchemes because, under the Australian Consumer Data Right, transport\n  and client authentication are defined by the CDR Security Profile\n  (FAPI 1.0 Advanced) separately from the resource-endpoint contract. This\n  profile records the two distinct authentication postures BankSA's CDR host\n  actually exposes.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  public_prd: none\n  oauth2_flows: [authorizationCode]\n  fapi_profile: FAPI 1.0 Advanced (CDR Security Profile)\nschemes:\n- name: PublicProductReferenceData\n  type: none\n  applies_to:\n  - GET /banking/products\n  - GET /banking/products/{productId}\n  description: >-\n    Product Reference Data (PRD) endpoints are mandated\
  \ by the CDR to be public\n    and unauthenticated. BankSA's live host returns HTTP 200 for these with no\n    Authorization header and no client certificate. A valid x-v version header\n    is still required (see conventions/banksa-conventions.yml).\n  sources: [openapi/banksa-cds-banking-products-openapi.yml]\n- name: CDRConsumerDataSharing\n  type: oauth2\n  scheme: FAPI 1.0 Advanced authorization-code with PAR + PKCE\n  description: >-\n    All consumer-data endpoints in this spec (accounts, balances, transactions,\n    direct debits, scheduled payments, payees) are only reachable by an\n    accredited data recipient (ADR) acting on a consumer's behalf. Authorization\n    uses OAuth 2.0 authorization-code with the OpenID Connect hybrid flow under\n    the FAPI 1.0 Advanced profile: Pushed Authorization Requests (PAR), PKCE,\n    request objects (JAR), and confirmation of the consumer's consent via the\n    CDR authorization server. Tokens are bound with mTLS sender-constrained\n  \
  \  access tokens.\n  flows:\n  - flow: authorizationCode\n    scopes: 9\n    detail: scopes/banksa-scopes.yml\n  sources: [openapi/banksa-cds-banking-products-openapi.yml]\n- name: CDRmTLS\n  type: mutualTLS\n  description: >-\n    The data-holder resource server is exposed on an mTLS endpoint (the OpenAPI\n    server is described as \"MTLS\"). Accredited data recipients present a client\n    certificate issued through the CDR Register PKI; access tokens are\n    sender-constrained (bound to the client certificate) per FAPI.\n  sources: [openapi/banksa-cds-banking-products-openapi.yml]\n- name: CDROpenIDConnect\n  type: openIdConnect\n  description: >-\n    Consumer authentication and consent are brokered through the data holder's\n    OpenID Provider, discovered by ADRs via the CDR Register rather than a public\n    /.well-known/openid-configuration on digital-api.banksa.com.au.\n  sources: [openapi/banksa-cds-banking-products-openapi.yml]\nnotes: >-\n  BankSA does not operate an independent\
  \ developer portal or issue self-service\n  API keys. There is no path to the consumer-data endpoints outside CDR\n  accreditation; the only openly consumable surface is the public PRD.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/authentication/banksa-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
