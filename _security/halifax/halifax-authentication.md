---
api_key_in: []
api_specs:
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data ATM Locator API
  slug: halifax-open-data-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Branch Locator API
  slug: halifax-open-data-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Personal Current Accounts API
  slug: halifax-open-data-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Business Current Accounts API
  slug: halifax-open-data-business-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Unsecured SME Loans API
  slug: halifax-open-data-unsecured-sme-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Commercial Credit Cards API
  slug: halifax-open-data-commercial-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
auth_types:
- none
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Halifax Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Halifax secures its APIs with none, oauth2, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Halifax
provider_slug: halifax
scheme_count: 4
schemes:
- flow: clientCredentials
  name: OAuth2 (client_credentials)
  scopes:
  - accounts
  - payments
  - fundsconfirmation
  sources:
  - OBIE Read/Write standard
  - developer.lloydsbanking.com
  type: oauth2
  used_for: Creating account-access-consent / payment-consent / funds-confirmation-consent resources.
- ciba_decoupled: true
  flow: authorizationCode
  name: OAuth2 (authorization_code)
  refresh_tokens: true
  scopes:
  - openid
  - accounts
  - payments
  - fundsconfirmation
  sources:
  - OBIE Read/Write standard
  - developer.lloydsbanking.com
  type: oauth2
  used_for: PSU authorises the consent; grants access + refresh token for data access / payment submission.
- detail: All Read/Write connections require mutual-TLS with an OBIE/eIDAS transport (QWAC) certificate. Lloyds supports tls_client_auth (mTLS client authentication) as an alternative to private_key_jwt client assertion.
  name: Mutual TLS
  sources:
  - developer.lloydsbanking.com
  type: mutualTLS
- detail: Supported client authentication method (JWS client assertion) alongside tls_client_auth.
  name: private_key_jwt
  type: oauth2-client-auth
slug: halifax-authentication
source_filename: halifax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.lloydsbanking.com/prod01/lbg/read-write\ndocs: https://openbankinguk.github.io/read-write-api-site3/v3.1.11/profiles/read-write-data-api-profile.html\nnote: >-\n  Two distinct auth postures. The OBIE Open Data APIs (ATM/branch/product\n  reference data) are PUBLIC and unauthenticated. The OBIE Read/Write APIs\n  (AIS/PIS/CBPII) are FAPI-secured and onboarded through the shared Lloyds\n  Banking Group Developer Portal. No OpenAPI securitySchemes were present in the\n  captured Open Data swagger, so this profile is sourced from the Lloyds portal\n  and the OBIE Read/Write standard rather than derived from a spec.\nsummary:\n  types: [none, oauth2, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\nsurfaces:\n  - name: OBIE Open Data APIs\n    apis:\n      - halifax-open-data-atm-locator-api\n      - halifax-open-data-branch-locator-api\n      - halifax-open-data-personal-current-accounts-api\n\
  \      - halifax-open-data-business-current-accounts-api\n      - halifax-open-data-unsecured-sme-loans-api\n      - halifax-open-data-commercial-credit-cards-api\n    auth: none\n    detail: Public, unauthenticated; TLS 1.2+ only. No credentials required.\n  - name: OBIE Read/Write APIs\n    apis:\n      - halifax-account-transaction-information-api\n      - halifax-payment-initiation-api\n      - halifax-confirmation-of-funds-api\n    auth: fapi\n    detail: >-\n      FAPI 1.0 Advanced. OAuth2/OIDC over mutual-TLS. TPPs onboard via the\n      Open Banking Directory and the Lloyds Banking Group Developer Portal\n      using OBIE/eIDAS (QWAC + QSeal) certificates.\nschemes:\n  - name: OAuth2 (client_credentials)\n    type: oauth2\n    flow: clientCredentials\n    used_for: Creating account-access-consent / payment-consent / funds-confirmation-consent resources.\n    scopes: [accounts, payments, fundsconfirmation]\n    sources: [OBIE Read/Write standard, developer.lloydsbanking.com]\n \
  \ - name: OAuth2 (authorization_code)\n    type: oauth2\n    flow: authorizationCode\n    used_for: PSU authorises the consent; grants access + refresh token for data access / payment submission.\n    scopes: [openid, accounts, payments, fundsconfirmation]\n    refresh_tokens: true\n    ciba_decoupled: true\n    sources: [OBIE Read/Write standard, developer.lloydsbanking.com]\n  - name: Mutual TLS\n    type: mutualTLS\n    detail: >-\n      All Read/Write connections require mutual-TLS with an OBIE/eIDAS transport\n      (QWAC) certificate. Lloyds supports tls_client_auth (mTLS client\n      authentication) as an alternative to private_key_jwt client assertion.\n    sources: [developer.lloydsbanking.com]\n  - name: private_key_jwt\n    type: oauth2-client-auth\n    detail: Supported client authentication method (JWS client assertion) alongside tls_client_auth.\nrequest_signing:\n  header: x-jws-signature\n  detail: Detached JWS signature over the request/response body for payment and consent\
  \ messages (OBIE message signing).\nrequired_headers:\n  - x-fapi-interaction-id\n  - x-fapi-auth-date\n  - x-fapi-customer-ip-address\n  - x-idempotency-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/authentication/halifax-authentication.yml
summary_line: none/oauth2/mutualTLS · 4 schemes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Open Data
---
