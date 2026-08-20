---
api_key_in: []
api_specs:
- filename: obie-open-data-api-standard-v1.3-swagger.json
  format: json
  label: Metro Bank Open Data API
  slug: metro-bank-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/obie-open-data-api-standard-v1.3-swagger.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Metro Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Metro Bank secures its APIs with oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Metro Bank
provider_slug: metro-bank
scheme_count: 4
schemes:
- applies_to:
  - metro-bank:metro-bank-open-data-api
  name: OpenData
  note: OBIE Open Data API standard defines no security scheme; access is public and read-only over HTTPS.
  scheme: public
  sources:
  - openapi/obie-open-data-api-standard-v1.3-swagger.json
  type: none
- applies_to:
  - metro-bank:metro-bank-account-information-api
  - metro-bank:metro-bank-payment-initiation-api
  - metro-bank:metro-bank-confirmation-of-funds-api
  fapi: true
  flows:
  - flow: authorizationCode
    note: Customer-present consent (PSD2 SCA) for AIS/PIS/CBPII resource access; OIDC hybrid flow with a signed request object (JWS), FAPI-compliant.
  - flow: clientCredentials
    note: Used to create the account-access / payment / funds-confirmation consent resource before the customer authorisation redirect.
  name: OBIE-FAPI-OAuth2
  sca: PSD2 strong customer authentication
  sources:
  - OBIE Read/Write API Security Profile
  type: oauth2
- applies_to:
  - metro-bank:metro-bank-account-information-api
  - metro-bank:metro-bank-payment-initiation-api
  - metro-bank:metro-bank-confirmation-of-funds-api
  name: OpenIDConnect
  note: OIDC provider issues id_token; discovery document is served from the ASPSP well-known endpoint (mTLS/edge-gated - not anonymously retrievable).
  type: openIdConnect
- applies_to:
  - metro-bank:metro-bank-account-information-api
  - metro-bank:metro-bank-payment-initiation-api
  - metro-bank:metro-bank-confirmation-of-funds-api
  name: MutualTLS
  note: Mandatory client-certificate transport security using eIDAS / OBIE (OBWAC / OBSEAL) certificates; also used for tls_client_auth token endpoint authentication. Confirmed live (HTTP 400 without a client cert).
  type: mutualTLS
slug: metro-bank-authentication
source_filename: metro-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  OBIE Read/Write API Security Profile (FAPI) + Metro Bank developer portal\n  (https://developer.metrobankonline.co.uk/Overview); Open Data API is\n  unauthenticated per the OBIE Open Data standard.\ndocs: https://developer.metrobankonline.co.uk/Overview\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  notes: >-\n    Two distinct auth postures. The OBIE Open Data reference API\n    (ATMs, branches, product data) is public and unauthenticated. The OBIE\n    Read/Write APIs (AIS, PIS, CBPII) are FAPI-secured and cannot be exercised\n    anonymously - the production host api.metrobankonline.co.uk enforces mutual\n    TLS (an unauthenticated request returns HTTP 400 \"No required SSL\n    certificate was sent\").\nschemes:\n  - name: OpenData\n    type: none\n    scheme: public\n    applies_to: [metro-bank:metro-bank-open-data-api]\n    sources:\
  \ [openapi/obie-open-data-api-standard-v1.3-swagger.json]\n    note: >-\n      OBIE Open Data API standard defines no security scheme; access is public\n      and read-only over HTTPS.\n  - name: OBIE-FAPI-OAuth2\n    type: oauth2\n    applies_to:\n      - metro-bank:metro-bank-account-information-api\n      - metro-bank:metro-bank-payment-initiation-api\n      - metro-bank:metro-bank-confirmation-of-funds-api\n    flows:\n      - flow: authorizationCode\n        note: >-\n          Customer-present consent (PSD2 SCA) for AIS/PIS/CBPII resource access;\n          OIDC hybrid flow with a signed request object (JWS), FAPI-compliant.\n      - flow: clientCredentials\n        note: >-\n          Used to create the account-access / payment / funds-confirmation\n          consent resource before the customer authorisation redirect.\n    fapi: true\n    sca: PSD2 strong customer authentication\n    sources: [OBIE Read/Write API Security Profile]\n  - name: OpenIDConnect\n    type: openIdConnect\n\
  \    applies_to:\n      - metro-bank:metro-bank-account-information-api\n      - metro-bank:metro-bank-payment-initiation-api\n      - metro-bank:metro-bank-confirmation-of-funds-api\n    note: >-\n      OIDC provider issues id_token; discovery document is served from the\n      ASPSP well-known endpoint (mTLS/edge-gated - not anonymously retrievable).\n  - name: MutualTLS\n    type: mutualTLS\n    applies_to:\n      - metro-bank:metro-bank-account-information-api\n      - metro-bank:metro-bank-payment-initiation-api\n      - metro-bank:metro-bank-confirmation-of-funds-api\n    note: >-\n      Mandatory client-certificate transport security using eIDAS / OBIE\n      (OBWAC / OBSEAL) certificates; also used for tls_client_auth token\n      endpoint authentication. Confirmed live (HTTP 400 without a client cert).\nclient_registration:\n  method: dynamic\n  standard: OBIE Dynamic Client Registration (DCR) with eIDAS/OBIE certificates\n  onboarding: >-\n    TPPs must onboard via the developer\
  \ portal and present valid OB certificates;\n    unregistered/anonymous access is not possible.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/authentication/metro-bank-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech
---
