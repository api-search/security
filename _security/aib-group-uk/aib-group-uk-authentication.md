---
api_key_in: []
api_specs:
- filename: aib-group-uk-atm-api-openapi.yml
  format: yaml
  label: AIB Group (UK) ATM API
  slug: aib-group-uk-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-atm-api-openapi.yml
- filename: aib-group-uk-bca-api-openapi.yml
  format: yaml
  label: AIB Group (UK) BCA API
  slug: aib-group-uk-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-bca-api-openapi.yml
- filename: aib-group-uk-branch-api-openapi.yml
  format: yaml
  label: AIB Group (UK) Branch API
  slug: aib-group-uk-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-branch-api-openapi.yml
- filename: aib-group-uk-ccc-api-openapi.yml
  format: yaml
  label: AIB Group (UK) CCC API
  slug: aib-group-uk-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-ccc-api-openapi.yml
- filename: aib-group-uk-pca-api-openapi.yml
  format: yaml
  label: AIB Group (UK) PCA API
  slug: aib-group-uk-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-pca-api-openapi.yml
- filename: aib-group-uk-sme-api-openapi.yml
  format: yaml
  label: AIB Group (UK) SME API
  slug: aib-group-uk-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-sme-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Aib Group Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: AIB Group (UK) secures its APIs with oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: AIB Group (UK)
provider_slug: aib-group-uk
scheme_count: 4
schemes:
- applies_to:
  - aib-group-uk-open-data-api
  description: Public, unauthenticated Open Data API (v2.2). No credentials required; product reference data served over TLS.
  name: OpenData
  type: none
- applies_to:
  - aib-group-uk-account-information-api
  - aib-group-uk-payment-initiation-api
  - aib-group-uk-confirmation-of-funds-api
  - aib-group-uk-variable-recurring-payments-api
  - aib-group-uk-credit-cards-information-api
  - aib-group-uk-event-notification-subscription-api
  - aib-group-uk-aggregated-event-polling-api
  description: OBIE FAPI-secured OAuth2 with OIDC. authorization_code (with PKCE / PAR / request object, JARM) for customer consent flows (AIS, PIS, CBPII, VRP); client_credentials for consent set-up. Access is granted through developer-portal onboarding and sandbox before production.
  flows:
  - description: Customer-present consent authorization (AIS/PIS/VRP/CBPII).
    flow: authorizationCode
  - description: Client-present consent set-up and event subscription.
    flow: clientCredentials
  name: OpenBankingOAuth2
  type: oauth2
- description: OpenID Connect identity layer over OAuth2 for the Read/Write APIs; id_token carries the consent and SCA assurance.
  name: OpenIDConnect
  type: openIdConnect
- applies_to:
  - aib-group-uk-dynamic-client-registration-api
  description: Mutual TLS with OBIE/eIDAS (QWAC/QSEAL) transport and signing certificates; required for Dynamic Client Registration (DCR v3.2) and token endpoints.
  name: MutualTLS
  type: mutualTLS
slug: aib-group-uk-authentication
source_filename: aib-group-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.aibgb.co.uk/apis\nnote: >-\n  AIB Group (UK) implements the UK Open Banking (OBIE) security profile. The\n  public Open Data API (v2.2) is unauthenticated. The Read/Write family\n  (Account Information, Payment Initiation, Confirmation of Funds, Variable\n  Recurring Payments, Event Notifications) is FAPI-secured under OAuth2/OIDC\n  with PSD2 strong customer authentication (SCA). TPPs onboard via OBIE Dynamic\n  Client Registration (DCR v3.2) using OBIE/eIDAS certificates. Access tokens\n  are obtained via authorization_code (customer-present, AIS/PIS consent) and\n  client_credentials (client-present setup) grants. The live OpenAPI spec\n  captured in this repo is the unauthenticated Open Data API and declares no\n  securitySchemes; the auth model below is captured from the developer portal\n  and OBIE standard, not derived from that spec.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in:\
  \ []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  strong_customer_authentication: true\n  standard: FAPI 1.0 Advanced (Financial-grade API) / OBIE Security Profile\nschemes:\n  - name: OpenData\n    type: none\n    description: >-\n      Public, unauthenticated Open Data API (v2.2). No credentials required;\n      product reference data served over TLS.\n    applies_to: [aib-group-uk-open-data-api]\n  - name: OpenBankingOAuth2\n    type: oauth2\n    description: >-\n      OBIE FAPI-secured OAuth2 with OIDC. authorization_code (with PKCE / PAR /\n      request object, JARM) for customer consent flows (AIS, PIS, CBPII, VRP);\n      client_credentials for consent set-up. Access is granted through\n      developer-portal onboarding and sandbox before production.\n    flows:\n      - flow: authorizationCode\n        description: Customer-present consent authorization (AIS/PIS/VRP/CBPII).\n      - flow: clientCredentials\n        description: Client-present consent set-up and event\
  \ subscription.\n    applies_to:\n      - aib-group-uk-account-information-api\n      - aib-group-uk-payment-initiation-api\n      - aib-group-uk-confirmation-of-funds-api\n      - aib-group-uk-variable-recurring-payments-api\n      - aib-group-uk-credit-cards-information-api\n      - aib-group-uk-event-notification-subscription-api\n      - aib-group-uk-aggregated-event-polling-api\n  - name: OpenIDConnect\n    type: openIdConnect\n    description: >-\n      OpenID Connect identity layer over OAuth2 for the Read/Write APIs; id_token\n      carries the consent and SCA assurance.\n  - name: MutualTLS\n    type: mutualTLS\n    description: >-\n      Mutual TLS with OBIE/eIDAS (QWAC/QSEAL) transport and signing certificates;\n      required for Dynamic Client Registration (DCR v3.2) and token endpoints.\n    applies_to: [aib-group-uk-dynamic-client-registration-api]\nonboarding:\n  model: self-serve developer portal + DCR\n  portal: https://developer.aibgb.co.uk/\n  dynamic_client_registration:\
  \ https://developer.aibgb.co.uk/dynamic-client-registration-api-v3-2-gb/apis\n  certificates: OBIE / eIDAS (QWAC, QSEAL)\n  sandbox: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/authentication/aib-group-uk-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Northern Ireland
---
