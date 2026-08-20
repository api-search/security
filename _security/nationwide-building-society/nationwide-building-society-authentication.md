---
api_key_in: []
api_specs:
- filename: obie-open-data-atm-locator-openapi.json
  format: json
  label: Nationwide ATM Locator API
  slug: nationwide-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-atm-locator-openapi.json
- filename: obie-open-data-branch-locator-openapi.json
  format: json
  label: Nationwide Branch Locator API
  slug: nationwide-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-branch-locator-openapi.json
- filename: obie-open-data-personal-current-accounts-openapi.json
  format: json
  label: Nationwide Personal Current Accounts API
  slug: nationwide-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-personal-current-accounts-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Nationwide Building Society Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Nationwide Building Society secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Nationwide Building Society
provider_slug: nationwide-building-society
scheme_count: 4
schemes:
- applies_to:
  - Nationwide ATM Locator API
  - Nationwide Branch Locator API
  - Nationwide Personal Current Accounts API
  name: OpenData
  note: Public, unauthenticated OBIE Open Data. No token or key required.
  tier: open-data
  type: none
- applies_to:
  - Nationwide Account and Transaction Information API (AIS)
  - Nationwide Payment Initiation API (PIS)
  - Nationwide Confirmation of Funds API (CBPII)
  - Nationwide Variable Recurring Payments API (VRP)
  flows:
  - flow: authorizationCode
    grant: authorization_code
    use: PSU consent authorisation (redirect + PSD2 SCA), used for AIS data access and payment authorisation
  - flow: clientCredentials
    grant: client_credentials
    use: TPP-only calls to create consent/intent resources before PSU authorisation
  name: OAuth2
  scheme: FAPI 1.0 Advanced
  scopes:
  - openid
  - accounts
  - payments
  - fundsconfirmations
  tier: read-write
  type: oauth2
- name: OpenIDConnect
  note: OIDC hybrid flow with request object (JWT), id_token, and the OBIE `intent` claim (openbanking_intent_id) carrying the consent id. Enforces PSD2 Strong Customer Authentication.
  tier: read-write
  type: openIdConnect
- confirmed: true
  evidence: TLS handshake to api.nationwide.co.uk returns "Request CERT" then fails without a presented client certificate (probed 2026-07-23).
  name: MutualTLS
  note: OBIE/eIDAS transport certificates (OBWAC/OBSeal or QWAC/QSeal) required for mutual-TLS client authentication and message signing; TPPs onboard via the developer portal and dynamic client registration.
  tier: read-write
  type: mutualTLS
slug: nationwide-building-society-authentication
source_filename: nationwide-building-society-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.nationwide.co.uk/open-banking\nstandard: OBIE Read/Write API Standard (FAPI 1.0 Advanced) + UK Open Banking Security Profile\ndocs: https://openbankinguk.github.io/read-write-api-site3/\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  notes: >-\n    Two distinct security tiers. The OBIE Open Data APIs (ATM/branch locators,\n    product reference data) are fully public and unauthenticated. The Read/Write\n    APIs (AIS/PIS/CBPII/VRP) require the full UK Open Banking FAPI security stack.\nschemes:\n- name: OpenData\n  tier: open-data\n  type: none\n  applies_to:\n  - Nationwide ATM Locator API\n  - Nationwide Branch Locator API\n  - Nationwide Personal Current Accounts API\n  note: Public, unauthenticated OBIE Open Data. No token or key required.\n- name: OAuth2\n  tier: read-write\n  type: oauth2\n  scheme: FAPI 1.0 Advanced\n\
  \  applies_to:\n  - Nationwide Account and Transaction Information API (AIS)\n  - Nationwide Payment Initiation API (PIS)\n  - Nationwide Confirmation of Funds API (CBPII)\n  - Nationwide Variable Recurring Payments API (VRP)\n  flows:\n  - flow: authorizationCode\n    grant: authorization_code\n    use: PSU consent authorisation (redirect + PSD2 SCA), used for AIS data access and payment authorisation\n  - flow: clientCredentials\n    grant: client_credentials\n    use: TPP-only calls to create consent/intent resources before PSU authorisation\n  scopes: [openid, accounts, payments, fundsconfirmations]\n- name: OpenIDConnect\n  tier: read-write\n  type: openIdConnect\n  note: >-\n    OIDC hybrid flow with request object (JWT), id_token, and the OBIE `intent`\n    claim (openbanking_intent_id) carrying the consent id. Enforces PSD2 Strong\n    Customer Authentication.\n- name: MutualTLS\n  tier: read-write\n  type: mutualTLS\n  confirmed: true\n  evidence: >-\n    TLS handshake to api.nationwide.co.uk\
  \ returns \"Request CERT\" then fails without\n    a presented client certificate (probed 2026-07-23).\n  note: >-\n    OBIE/eIDAS transport certificates (OBWAC/OBSeal or QWAC/QSeal) required for\n    mutual-TLS client authentication and message signing; TPPs onboard via the\n    developer portal and dynamic client registration.\nmessage_signing:\n  header: x-jws-signature\n  note: Detached JWS signature required on payment/consent write operations per the OBIE profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/authentication/nationwide-building-society-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial-Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
---
