---
api_key_in: []
api_specs:
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Product Reference Data API
  slug: great-southern-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank Business+ CDR Product Reference Data API
  slug: great-southern-bank-business-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Accounts & Balances API
  slug: great-southern-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Transactions API
  slug: great-southern-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Direct Debits & Scheduled Payments API
  slug: great-southern-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Payees API
  slug: great-southern-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Great Southern Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Great Southern Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Great Southern Bank
provider_slug: great-southern-bank
scheme_count: 4
schemes:
- applies_to:
  - listBankingProducts
  - getBankingProductDetail
  name: PublicProductReferenceData
  note: 'Product Reference Data endpoints are openly accessible with no credential. Confirmed live: GET https://api.open-banking.greatsouthernbank.com.au/cds-au/v1/banking/products returns HTTP 200 with no Authorization header.'
  sources:
  - openapi/great-southern-bank-cds-banking-products-openapi.yml
  type: none
- applies_to: authenticated CDR banking resource endpoints (ADR-only)
  name: CDR-OIDC-FAPI
  note: 'Consumer data sharing follows the CDR security profile: OpenID Connect with the FAPI 1.0 Advanced profile, Pushed Authorization Requests (PAR), private_key_jwt client authentication, and the CDR Register''s dynamic client registration and ADR accreditation model. Not available to the general public.'
  scheme: fapi-1.0-advanced
  sources:
  - review.yml
  type: openIdConnect
- applies_to: authenticated CDR banking resource endpoints (ADR-only)
  flows:
  - flow: authorizationCode
    note: Authorization Code flow with PKCE per the CDR / FAPI security profile; consumer authorises data sharing.
  name: CDR-OAuth2
  scopes:
  - bank:accounts.basic:read
  - bank:accounts.detail:read
  - bank:transactions:read
  - bank:payees:read
  - bank:regular_payments:read
  sources:
  - openapi/great-southern-bank-cds-banking-products-openapi.yml
  type: oauth2
- applies_to: all authenticated CDR data-holder endpoints
  name: MutualTLS
  note: CDR data-holder endpoints are served over the MTLS server described in the spec (servers[].description "MTLS"); ADRs present a CDR-issued client certificate.
  sources:
  - openapi/great-southern-bank-cds-banking-products-openapi.yml
  type: mutualTLS
slug: great-southern-bank-authentication
source_filename: great-southern-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://www.greatsouthernbank.com.au/consumer-data-policy\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  note: >-\n    The only public, self-serve surface at Great Southern Bank is the Consumer\n    Data Right (CDR) Product Reference Data (PRD) API, which is UNAUTHENTICATED\n    by standard (no API key, no token). All other CDR banking resource endpoints\n    (accounts, balances, transactions, direct debits, scheduled payments, payees)\n    are authenticated under the CDR security profile and are reachable ONLY by\n    ACCC-accredited data recipients (ADRs). The bank does not issue self-service\n    API keys and operates no public developer portal.\ndiscovery:\n  source: https://secure.open-banking.greatsouthernbank.com.au/.well-known/openid-configuration\n  confirmed: '2026-07-21'\n  issuer: https://auth.open-banking.greatsouthernbank.com.au\n\
  \  authorization_endpoint: https://secure.open-banking.greatsouthernbank.com.au/as/authorization.oauth2\n  token_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/token.oauth2\n  pushed_authorization_request_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/par.oauth2\n  registration_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/clients.oauth2\n  backchannel_authentication_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/bc-auth.ciba\n  cdr_arrangement_revocation_endpoint: https://auth.open-banking.greatsouthernbank.com.au/data-holder/arrangements/revoke\n  require_pushed_authorization_requests: true\n  tls_client_certificate_bound_access_tokens: true\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt]\n  code_challenge_methods_supported: [S256]\n  acr_values_supported: [urn:cds.au:cdr:2]\n  id_token_signing_alg_values_supported: [ES256, PS256]\n  grant_types_supported: [authorization_code,\
  \ client_credentials, refresh_token]\nschemes:\n- name: PublicProductReferenceData\n  type: none\n  applies_to:\n  - listBankingProducts\n  - getBankingProductDetail\n  note: >-\n    Product Reference Data endpoints are openly accessible with no credential.\n    Confirmed live: GET https://api.open-banking.greatsouthernbank.com.au/cds-au/v1/banking/products\n    returns HTTP 200 with no Authorization header.\n  sources:\n  - openapi/great-southern-bank-cds-banking-products-openapi.yml\n- name: CDR-OIDC-FAPI\n  type: openIdConnect\n  scheme: fapi-1.0-advanced\n  applies_to: authenticated CDR banking resource endpoints (ADR-only)\n  note: >-\n    Consumer data sharing follows the CDR security profile: OpenID Connect with\n    the FAPI 1.0 Advanced profile, Pushed Authorization Requests (PAR), private_key_jwt\n    client authentication, and the CDR Register's dynamic client registration and\n    ADR accreditation model. Not available to the general public.\n  sources:\n  - review.yml\n- name:\
  \ CDR-OAuth2\n  type: oauth2\n  applies_to: authenticated CDR banking resource endpoints (ADR-only)\n  flows:\n  - flow: authorizationCode\n    note: Authorization Code flow with PKCE per the CDR / FAPI security profile; consumer authorises data sharing.\n  scopes:\n  - bank:accounts.basic:read\n  - bank:accounts.detail:read\n  - bank:transactions:read\n  - bank:payees:read\n  - bank:regular_payments:read\n  sources:\n  - openapi/great-southern-bank-cds-banking-products-openapi.yml\n- name: MutualTLS\n  type: mutualTLS\n  applies_to: all authenticated CDR data-holder endpoints\n  note: >-\n    CDR data-holder endpoints are served over the MTLS server described in the\n    spec (servers[].description \"MTLS\"); ADRs present a CDR-issued client certificate.\n  sources:\n  - openapi/great-southern-bank-cds-banking-products-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/authentication/great-southern-bank-authentication.yml
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
