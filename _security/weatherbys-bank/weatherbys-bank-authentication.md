---
api_key_in: []
api_specs:
- filename: weatherbys-bank-atm-api-openapi.yml
  format: yaml
  label: Weatherbys Bank ATM API
  slug: weatherbys-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-atm-api-openapi.yml
- filename: weatherbys-bank-bca-api-openapi.yml
  format: yaml
  label: Weatherbys Bank BCA API
  slug: weatherbys-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-bca-api-openapi.yml
- filename: weatherbys-bank-branch-api-openapi.yml
  format: yaml
  label: Weatherbys Bank Branch API
  slug: weatherbys-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-branch-api-openapi.yml
- filename: weatherbys-bank-pca-api-openapi.yml
  format: yaml
  label: Weatherbys Bank PCA API
  slug: weatherbys-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-pca-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Weatherbys Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Weatherbys Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Weatherbys Bank
provider_slug: weatherbys-bank
scheme_count: 4
schemes:
- applies_to:
  - ATM Locator
  - Branch Locator
  - Personal Current Accounts
  - Business Current Accounts
  name: open-data-public
  type: none
- applies_to:
  - AIS
  - PIS
  - CBPII
  flows:
  - authorizationCode
  - clientCredentials
  name: fapi-oauth2
  scopes_ref: scopes/weatherbys-bank-scopes.yml
  transport: mutual-TLS (FAPI 1.0 Advanced)
  type: oauth2
- applies_to:
  - AIS
  - PIS
  - CBPII
  detail: OpenID Connect hybrid flow with request object (JWT), PSD2 SCA
  name: fapi-oidc
  type: openIdConnect
- applies_to:
  - AIS
  - PIS
  - CBPII
  detail: OBIE/eIDAS transport (OBWAC) + signing (OBSeal) certificates
  name: mutual-tls
  type: mutualTLS
slug: weatherbys-bank-authentication
source_filename: weatherbys-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://openbankinguk.github.io/read-write-api-site3/ (OBIE Read/Write + Open Data standards)\ndocs: https://www.openbanking.org.uk/regulated-providers/weatherbys-bank-limited/\nnote: >-\n  Two distinct auth profiles. (1) The Open Data APIs (ATM/Branch locators,\n  personal/business current account product data) are PUBLIC and unauthenticated —\n  no security scheme. (2) The Read/Write APIs (AIS/PIS/CBPII) are FAPI-secured per\n  the OBIE Read/Write standard this ASPSP conforms to as an FCA-authorised\n  participant in UK Open Banking: OAuth2 + OpenID Connect over mutual-TLS, with\n  PSD2 Strong Customer Authentication. Client onboarding requires OBIE/eIDAS\n  (OBWAC/OBSeal) certificates and OpenID dynamic client registration. Credentials\n  are provider-issued and are not fabricated here.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  open_data_auth: none\n  read_write_auth: [oauth2, openIdConnect, mutualTLS]\n\
  \  oauth2_flows: [authorizationCode, clientCredentials]\n  client_auth_methods: [tls_client_auth, private_key_jwt]\nschemes:\n- name: open-data-public\n  type: none\n  applies_to: [ATM Locator, Branch Locator, Personal Current Accounts, Business Current Accounts]\n- name: fapi-oauth2\n  type: oauth2\n  flows: [authorizationCode, clientCredentials]\n  transport: mutual-TLS (FAPI 1.0 Advanced)\n  applies_to: [AIS, PIS, CBPII]\n  scopes_ref: scopes/weatherbys-bank-scopes.yml\n- name: fapi-oidc\n  type: openIdConnect\n  detail: OpenID Connect hybrid flow with request object (JWT), PSD2 SCA\n  applies_to: [AIS, PIS, CBPII]\n- name: mutual-tls\n  type: mutualTLS\n  detail: OBIE/eIDAS transport (OBWAC) + signing (OBSeal) certificates\n  applies_to: [AIS, PIS, CBPII]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/authentication/weatherbys-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Private Banking
---
