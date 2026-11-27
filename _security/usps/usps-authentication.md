---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usps-addresses-api-openapi.yml
  format: yaml
  label: United States Postal Service Addresses API
  slug: usps-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-addresses-api-openapi.yml
- filename: usps-carrier-pickup-api-openapi.yml
  format: yaml
  label: United States Postal Service Carrier Pickup API
  slug: usps-carrier-pickup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-carrier-pickup-api-openapi.yml
- filename: usps-domestic-prices-api-openapi.yml
  format: yaml
  label: United States Postal Service Domestic Prices API
  slug: usps-domestic-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-domestic-prices-api-openapi.yml
- filename: usps-files-api-openapi.yml
  format: yaml
  label: United States Postal Service Files API
  slug: usps-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-files-api-openapi.yml
- filename: usps-listener-url-specification-api-openapi.yml
  format: yaml
  label: United States Postal Service Listener URL Specification API
  slug: usps-listener-url-specification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-listener-url-specification-api-openapi.yml
- filename: usps-resources-api-openapi.yml
  format: yaml
  label: United States Postal Service Resources API
  slug: usps-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-resources-api-openapi.yml
- filename: usps-tracking-api-openapi.yml
  format: yaml
  label: United States Postal Service Tracking API
  slug: usps-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-tracking-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: United States Postal Service Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: United States Postal Service secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: United States Postal Service
provider_slug: usps
scheme_count: 4
schemes:
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /oauth2/v3/token
  name: OAuth
  sources:
  - openapi/usps-addresses-openapi.yml
  - openapi/usps-adjustments-openapi.yml
  - openapi/usps-appointments-openapi.yml
  - openapi/usps-carrier-pickup-openapi.yml
  - openapi/usps-domestic-labels-openapi.yml
  - openapi/usps-domestic-prices-openapi.yml
  - openapi/usps-international-labels-openapi.yml
  - openapi/usps-international-prices-openapi.yml
  - openapi/usps-locations-openapi.yml
  - openapi/usps-logistics-shipments-openapi.yml
  - openapi/usps-ncoa-openapi.yml
  - openapi/usps-pmod-openapi.yml
  - openapi/usps-qr-codes-openapi.yml
  - openapi/usps-reconciliation-adjustments-openapi.yml
  - openapi/usps-scan-forms-openapi.yml
  - openapi/usps-service-standards-files-openapi.yml
  - openapi/usps-service-standards-openapi.yml
  - openapi/usps-ship-enrollment-openapi.yml
  - openapi/usps-subscriptions-addresses-openapi.yml
  - openapi/usps-subscriptions-adjustments-openapi.yml
  - openapi/usps-subscriptions-disputes-openapi.yml
  - openapi/usps-subscriptions-ncoa-openapi.yml
  - openapi/usps-subscriptions-package-transaction-details-openapi.yml
  - openapi/usps-subscriptions-tracking-openapi.yml
  - openapi/usps-subscriptions-tracking-v3r2-openapi.yml
  - openapi/usps-subscriptions-unpaid-packages-openapi.yml
  - openapi/usps-tracking-openapi.yml
  - openapi/usps-tracking-v3r2-openapi.yml
  - openapi/usps-userinfo-openapi.yml
  type: oauth2
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /oauth2/v3/token
  name: OAuth
  sources:
  - openapi/usps-containers-openapi.yml
  - openapi/usps-informed-delivery-mail-campaigns-openapi.yml
  - openapi/usps-informed-delivery-package-campaigns-openapi.yml
  - openapi/usps-international-service-standards-openapi.yml
  - openapi/usps-payments-openapi.yml
  - openapi/usps-service-standards-directory-openapi.yml
  - openapi/usps-shipping-options-openapi.yml
  type: oauth2
- description: Use the client_id and client_secret for the username and password, respectfully. The client application is authenticated using the Basic authentication security scheme.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/usps-oauth-openapi.yml
  type: http
- bearerFormat: JWT
  description: An access token is used to authenticate the client application making the request.
  name: BearerTokenAuth
  scheme: bearer
  sources:
  - openapi/usps-oauth-openapi.yml
  type: http
slug: usps-authentication
source_filename: usps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://developers.usps.com/getting-started; openapi/usps-addresses-openapi.yml, openapi/usps-adjustments-openapi.yml,\n  openapi/usps-appointments-openapi.yml, openapi/usps-carrier-pickup-openapi.yml, openapi/usps-containers-openapi.yml, openapi/usps-domestic-labels-openapi.yml,\n  openapi/usps-domestic-prices-openapi.yml, openapi/usps-informed-delivery-mail-campaigns-openapi.yml, openapi/usps-informed-delivery-package-campaigns-openapi.yml,\n  openapi/usps-international-labels-openapi.yml, openapi/usps-international-prices-openapi.yml, openapi/usps-international-service-standards-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n\
  \    scopes: 1\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version\n    3 API which supplies this access token is provided below for reference.\n  sources:\n  - openapi/usps-addresses-openapi.yml\n  - openapi/usps-adjustments-openapi.yml\n  - openapi/usps-appointments-openapi.yml\n  - openapi/usps-carrier-pickup-openapi.yml\n  - openapi/usps-domestic-labels-openapi.yml\n  - openapi/usps-domestic-prices-openapi.yml\n  - openapi/usps-international-labels-openapi.yml\n  - openapi/usps-international-prices-openapi.yml\n  - openapi/usps-locations-openapi.yml\n  - openapi/usps-logistics-shipments-openapi.yml\n  - openapi/usps-ncoa-openapi.yml\n  - openapi/usps-pmod-openapi.yml\n  - openapi/usps-qr-codes-openapi.yml\n  - openapi/usps-reconciliation-adjustments-openapi.yml\n  - openapi/usps-scan-forms-openapi.yml\n  - openapi/usps-service-standards-files-openapi.yml\n  - openapi/usps-service-standards-openapi.yml\n  -\
  \ openapi/usps-ship-enrollment-openapi.yml\n  - openapi/usps-subscriptions-addresses-openapi.yml\n  - openapi/usps-subscriptions-adjustments-openapi.yml\n  - openapi/usps-subscriptions-disputes-openapi.yml\n  - openapi/usps-subscriptions-ncoa-openapi.yml\n  - openapi/usps-subscriptions-package-transaction-details-openapi.yml\n  - openapi/usps-subscriptions-tracking-openapi.yml\n  - openapi/usps-subscriptions-tracking-v3r2-openapi.yml\n  - openapi/usps-subscriptions-unpaid-packages-openapi.yml\n  - openapi/usps-tracking-openapi.yml\n  - openapi/usps-tracking-v3r2-openapi.yml\n  - openapi/usps-userinfo-openapi.yml\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n    scopes: 1\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version\n    3 API which supplies this access token is provided below for reference.\n  sources:\n  - openapi/usps-containers-openapi.yml\n  -\
  \ openapi/usps-informed-delivery-mail-campaigns-openapi.yml\n  - openapi/usps-informed-delivery-package-campaigns-openapi.yml\n  - openapi/usps-international-service-standards-openapi.yml\n  - openapi/usps-payments-openapi.yml\n  - openapi/usps-service-standards-directory-openapi.yml\n  - openapi/usps-shipping-options-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Use the client_id and client_secret for the username and password, respectfully. The client application is\n    authenticated using the Basic authentication security scheme.\n  sources:\n  - openapi/usps-oauth-openapi.yml\n- name: BearerTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: An access token is used to authenticate the client application making the request.\n  sources:\n  - openapi/usps-oauth-openapi.yml\ndocs: https://developers.usps.com/getting-started\ndocs_summary: Create an app in the USPS Customer Onboarding Portal (COP); pass its Consumer Key and Consumer\
  \ Secret as client_id\n  and client_secret to the OAuth API; all USPS APIs require the token in the Authorization header using the Bearer Token scheme.\n  Labels APIs additionally take an X-Payment-Authorization-Token from the Payments API.\n"
source_yaml_url: https://artifacts.apis.io/usps/authentication/usps-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Government
- Postal Service
- Shipping
- Logistics
- Address Validation
- Package Tracking
---
