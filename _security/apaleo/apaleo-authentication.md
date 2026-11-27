---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apaleo-booking-api-openapi.yml
  format: yaml
  label: apaleo Booking API
  slug: apaleo-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-booking-api-openapi.yml
- filename: apaleo-authorization-api-openapi.yml
  format: yaml
  label: apaleo Authorization API
  slug: apaleo-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-authorization-api-openapi.yml
- filename: apaleo-authorizationactions-api-openapi.yml
  format: yaml
  label: apaleo Authorization Actions API
  slug: apaleo-authorizationactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-authorizationactions-api-openapi.yml
- filename: apaleo-block-api-openapi.yml
  format: yaml
  label: apaleo Block API
  slug: apaleo-block-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-block-api-openapi.yml
- filename: apaleo-blockactions-api-openapi.yml
  format: yaml
  label: apaleo Block Actions API
  slug: apaleo-blockactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-blockactions-api-openapi.yml
- filename: apaleo-group-api-openapi.yml
  format: yaml
  label: apaleo Group API
  slug: apaleo-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-group-api-openapi.yml
- filename: apaleo-groupactions-api-openapi.yml
  format: yaml
  label: apaleo Group Actions API
  slug: apaleo-groupactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-groupactions-api-openapi.yml
- filename: apaleo-offer-api-openapi.yml
  format: yaml
  label: apaleo Offer API
  slug: apaleo-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-offer-api-openapi.yml
- filename: apaleo-paymentaccountactions-api-openapi.yml
  format: yaml
  label: apaleo Payment Account Actions API
  slug: apaleo-paymentaccountactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-paymentaccountactions-api-openapi.yml
- filename: apaleo-reservation-api-openapi.yml
  format: yaml
  label: apaleo Reservation API
  slug: apaleo-reservation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-reservation-api-openapi.yml
- filename: apaleo-reservationactions-api-openapi.yml
  format: yaml
  label: apaleo Reservation Actions API
  slug: apaleo-reservationactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-reservationactions-api-openapi.yml
- filename: apaleo-types-api-openapi.yml
  format: yaml
  label: apaleo Types API
  slug: apaleo-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-types-api-openapi.yml
- filename: apaleo-payment-account-api-openapi.yml
  format: yaml
  label: apaleo Payment Account API
  slug: apaleo-payment-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-payment-account-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: apaleo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: apaleo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: apaleo
provider_slug: apaleo
scheme_count: 1
schemes:
- description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials and authorization-code grants are supported.
  flows:
  - flow: clientCredentials
    scopes: 10
    tokenUrl: https://identity.apaleo.com/connect/token
  - authorizationUrl: https://identity.apaleo.com/connect/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://identity.apaleo.com/connect/token
  name: oauth2
  sources:
  - openapi/apaleo-openapi.yml
  type: oauth2
slug: apaleo-authentication
source_filename: apaleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apaleo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.apaleo.com/connect/token\n    scopes: 10\n  - flow: authorizationCode\n    authorizationUrl: https://identity.apaleo.com/connect/authorize\n    tokenUrl: https://identity.apaleo.com/connect/token\n    scopes: 10\n  description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity\n    provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials\n    and authorization-code grants are supported.\n  sources:\n  - openapi/apaleo-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/apaleo/authentication/apaleo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Hospitality
- PMS
- Property Management
- Hotels
- API-First
---
