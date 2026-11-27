---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-wallet-jwt-api-openapi.yml
  format: yaml
  label: Google Wallet JWT API
  slug: google-wallet-jwt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-jwt-api-openapi.yml
- filename: google-wallet-eventticketclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Eventticketclass API
  slug: google-wallet-eventticketclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-eventticketclass-api-openapi.yml
- filename: google-wallet-eventticketobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Eventticketobject API
  slug: google-wallet-eventticketobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-eventticketobject-api-openapi.yml
- filename: google-wallet-flightclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Flightclass API
  slug: google-wallet-flightclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-flightclass-api-openapi.yml
- filename: google-wallet-flightobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Flightobject API
  slug: google-wallet-flightobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-flightobject-api-openapi.yml
- filename: google-wallet-genericclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Genericclass API
  slug: google-wallet-genericclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-genericclass-api-openapi.yml
- filename: google-wallet-genericobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Genericobject API
  slug: google-wallet-genericobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-genericobject-api-openapi.yml
- filename: google-wallet-giftcardclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Giftcardclass API
  slug: google-wallet-giftcardclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-giftcardclass-api-openapi.yml
- filename: google-wallet-giftcardobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Giftcardobject API
  slug: google-wallet-giftcardobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-giftcardobject-api-openapi.yml
- filename: google-wallet-issuer-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Issuer API
  slug: google-wallet-issuer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-issuer-api-openapi.yml
- filename: google-wallet-loyaltyclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Loyaltyclass API
  slug: google-wallet-loyaltyclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-loyaltyclass-api-openapi.yml
- filename: google-wallet-loyaltyobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Loyaltyobject API
  slug: google-wallet-loyaltyobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-loyaltyobject-api-openapi.yml
- filename: google-wallet-media-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Media API
  slug: google-wallet-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-media-api-openapi.yml
- filename: google-wallet-offerclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Offerclass API
  slug: google-wallet-offerclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-offerclass-api-openapi.yml
- filename: google-wallet-offerobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Offerobject API
  slug: google-wallet-offerobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-offerobject-api-openapi.yml
- filename: google-wallet-permissions-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Permissions API
  slug: google-wallet-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-permissions-api-openapi.yml
- filename: google-wallet-smarttap-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Smarttap API
  slug: google-wallet-smarttap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-smarttap-api-openapi.yml
- filename: google-wallet-transitclass-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Transitclass API
  slug: google-wallet-transitclass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-transitclass-api-openapi.yml
- filename: google-wallet-transitobject-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Transitobject API
  slug: google-wallet-transitobject-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-transitobject-api-openapi.yml
- filename: google-wallet-walletobjects-api-openapi.yml
  format: yaml
  label: Google Wallet Wallet Walletobjects API
  slug: google-wallet-walletobjects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-wallet/openapi/google-wallet-walletobjects-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Wallet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Wallet secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Wallet
provider_slug: google-wallet
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-wallet-eventticketclass-api-openapi.yml
  - openapi/google-wallet-eventticketobject-api-openapi.yml
  - openapi/google-wallet-flightclass-api-openapi.yml
  - openapi/google-wallet-flightobject-api-openapi.yml
  - openapi/google-wallet-genericclass-api-openapi.yml
  - openapi/google-wallet-genericobject-api-openapi.yml
  - openapi/google-wallet-giftcardclass-api-openapi.yml
  - openapi/google-wallet-giftcardobject-api-openapi.yml
  - openapi/google-wallet-issuer-api-openapi.yml
  - openapi/google-wallet-jwt-api-openapi.yml
  - openapi/google-wallet-loyaltyclass-api-openapi.yml
  - openapi/google-wallet-loyaltyobject-api-openapi.yml
  - openapi/google-wallet-media-api-openapi.yml
  - openapi/google-wallet-offerclass-api-openapi.yml
  - openapi/google-wallet-offerobject-api-openapi.yml
  - openapi/google-wallet-permissions-api-openapi.yml
  - openapi/google-wallet-smarttap-api-openapi.yml
  - openapi/google-wallet-transitclass-api-openapi.yml
  - openapi/google-wallet-transitobject-api-openapi.yml
  - openapi/google-wallet-walletobjects-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-wallet-eventticketclass-api-openapi.yml
  - openapi/google-wallet-eventticketobject-api-openapi.yml
  - openapi/google-wallet-flightclass-api-openapi.yml
  - openapi/google-wallet-flightobject-api-openapi.yml
  - openapi/google-wallet-genericclass-api-openapi.yml
  - openapi/google-wallet-genericobject-api-openapi.yml
  - openapi/google-wallet-giftcardclass-api-openapi.yml
  - openapi/google-wallet-giftcardobject-api-openapi.yml
  - openapi/google-wallet-issuer-api-openapi.yml
  - openapi/google-wallet-jwt-api-openapi.yml
  - openapi/google-wallet-loyaltyclass-api-openapi.yml
  - openapi/google-wallet-loyaltyobject-api-openapi.yml
  - openapi/google-wallet-media-api-openapi.yml
  - openapi/google-wallet-offerclass-api-openapi.yml
  - openapi/google-wallet-offerobject-api-openapi.yml
  - openapi/google-wallet-permissions-api-openapi.yml
  - openapi/google-wallet-smarttap-api-openapi.yml
  - openapi/google-wallet-transitclass-api-openapi.yml
  - openapi/google-wallet-transitobject-api-openapi.yml
  - openapi/google-wallet-walletobjects-api-openapi.yml
  type: oauth2
slug: google-wallet-authentication
source_filename: google-wallet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-wallet-eventticketclass-api-openapi.yml, openapi/google-wallet-eventticketobject-api-openapi.yml,\n  openapi/google-wallet-flightclass-api-openapi.yml, openapi/google-wallet-flightobject-api-openapi.yml,\n  openapi/google-wallet-genericclass-api-openapi.yml, openapi/google-wallet-genericobject-api-openapi.yml,\n  openapi/google-wallet-giftcardclass-api-openapi.yml, openapi/google-wallet-giftcardobject-api-openapi.yml,\n  openapi/google-wallet-issuer-api-openapi.yml, openapi/google-wallet-jwt-api-openapi.yml, openapi/google-wallet-loyaltyclass-api-openapi.yml,\n  openapi/google-wallet-loyaltyobject-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-wallet-eventticketclass-api-openapi.yml\n\
  \  - openapi/google-wallet-eventticketobject-api-openapi.yml\n  - openapi/google-wallet-flightclass-api-openapi.yml\n  - openapi/google-wallet-flightobject-api-openapi.yml\n  - openapi/google-wallet-genericclass-api-openapi.yml\n  - openapi/google-wallet-genericobject-api-openapi.yml\n  - openapi/google-wallet-giftcardclass-api-openapi.yml\n  - openapi/google-wallet-giftcardobject-api-openapi.yml\n  - openapi/google-wallet-issuer-api-openapi.yml\n  - openapi/google-wallet-jwt-api-openapi.yml\n  - openapi/google-wallet-loyaltyclass-api-openapi.yml\n  - openapi/google-wallet-loyaltyobject-api-openapi.yml\n  - openapi/google-wallet-media-api-openapi.yml\n  - openapi/google-wallet-offerclass-api-openapi.yml\n  - openapi/google-wallet-offerobject-api-openapi.yml\n  - openapi/google-wallet-permissions-api-openapi.yml\n  - openapi/google-wallet-smarttap-api-openapi.yml\n  - openapi/google-wallet-transitclass-api-openapi.yml\n  - openapi/google-wallet-transitobject-api-openapi.yml\n  - openapi/google-wallet-walletobjects-api-openapi.yml\n\
  - name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/google-wallet-eventticketclass-api-openapi.yml\n  - openapi/google-wallet-eventticketobject-api-openapi.yml\n  - openapi/google-wallet-flightclass-api-openapi.yml\n  - openapi/google-wallet-flightobject-api-openapi.yml\n  - openapi/google-wallet-genericclass-api-openapi.yml\n  - openapi/google-wallet-genericobject-api-openapi.yml\n  - openapi/google-wallet-giftcardclass-api-openapi.yml\n  - openapi/google-wallet-giftcardobject-api-openapi.yml\n  - openapi/google-wallet-issuer-api-openapi.yml\n  - openapi/google-wallet-jwt-api-openapi.yml\n  - openapi/google-wallet-loyaltyclass-api-openapi.yml\n  - openapi/google-wallet-loyaltyobject-api-openapi.yml\n  - openapi/google-wallet-media-api-openapi.yml\n  - openapi/google-wallet-offerclass-api-openapi.yml\n  - openapi/google-wallet-offerobject-api-openapi.yml\n\
  \  - openapi/google-wallet-permissions-api-openapi.yml\n  - openapi/google-wallet-smarttap-api-openapi.yml\n  - openapi/google-wallet-transitclass-api-openapi.yml\n  - openapi/google-wallet-transitobject-api-openapi.yml\n  - openapi/google-wallet-walletobjects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-wallet/authentication/google-wallet-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Digital Wallet
- Google Wallet
- Loyalty Cards
- Mobile Payments
- Passes
- Ticketing
---
