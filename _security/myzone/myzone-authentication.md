---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myzone-accounts-api-openapi.yml
  format: yaml
  label: Myzone Accounts API
  slug: myzone-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-accounts-api-openapi.yml
- filename: myzone-biometrics-api-openapi.yml
  format: yaml
  label: Myzone Biometrics API
  slug: myzone-biometrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-biometrics-api-openapi.yml
- filename: myzone-challenges-api-openapi.yml
  format: yaml
  label: Myzone Challenges API
  slug: myzone-challenges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-challenges-api-openapi.yml
- filename: myzone-classes-and-booking-api-openapi.yml
  format: yaml
  label: Myzone Classes And Booking API
  slug: myzone-classes-and-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-classes-and-booking-api-openapi.yml
- filename: myzone-facilities-api-openapi.yml
  format: yaml
  label: Myzone Facilities API
  slug: myzone-facilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-facilities-api-openapi.yml
- filename: myzone-groups-api-openapi.yml
  format: yaml
  label: Myzone Groups API
  slug: myzone-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-groups-api-openapi.yml
- filename: myzone-moves-api-openapi.yml
  format: yaml
  label: Myzone Moves API
  slug: myzone-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-moves-api-openapi.yml
- filename: myzone-reports-api-openapi.yml
  format: yaml
  label: Myzone Reports API
  slug: myzone-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-reports-api-openapi.yml
- filename: myzone-webhooks-api-openapi.yml
  format: yaml
  label: Myzone Webhooks API
  slug: myzone-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-webhooks-api-openapi.yml
auth_types: []
description: 'Myzone supports OAuth 2.0 authentication with two grant types: Client Credentials and Authorization Code Flow with PKCE.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Myzone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Myzone declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Myzone
provider_slug: myzone
scheme_count: 1
schemes:
- evidence: 'We support **two OAuth 2.0 grant types** for API authorization, each designed for different use cases:'
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: Obtain a client ID and client secret from Myzone, then request an access token from the token URL using the appropriate grant type.
  name: OAuth 2.0
  scopes:
  - read:accounts
  - write:accounts
  - delete:accounts
  - read:moves
  - read:moves:hr
  - read:biometrics
  - write:biometrics
  - read:classes_and_bookings
  - write:classes_and_bookings
  - delete:classes_and_bookings
  - read:challenges
  - read:facilities
  - read:reports
  - read:groups
  - write:groups
  - delete:groups
  - read:webhooks
  - write:webhooks
  - delete:webhooks
  token_url: https://auth.myzone.org/access_token
  type: oauth2
slug: myzone-authentication
source_filename: myzone-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.myzone.org/reference/oauth-20-grant-types.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.myzone.org/reference/oauth-20-grant-types.md\nsources:\n- https://docs.myzone.org/reference/oauth-20-grant-types.md\n- https://docs.myzone.org/recipes/oauth-20-authentication-with-javascript.md\n- https://docs.myzone.org/reference/oauth-20-grant-types\n- https://docs.myzone.org/reference/oauth-20-grant-types\ndescription: 'Myzone supports OAuth 2.0 authentication with two grant types: Client Credentials and Authorization Code Flow with PKCE.'\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'We support **two OAuth 2.0 grant types** for API authorization, each designed for different use cases:'\n  flows:\n  - client_credentials\n  - authorization_code\n  token_url: https://auth.myzone.org/access_token\n  scopes:\n  - read:accounts\n  - write:accounts\n  - delete:accounts\n  - read:moves\n  - read:moves:hr\n  - read:biometrics\n  - write:biometrics\n  - read:classes_and_bookings\n\
  \  - write:classes_and_bookings\n  - delete:classes_and_bookings\n  - read:challenges\n  - read:facilities\n  - read:reports\n  - read:groups\n  - write:groups\n  - delete:groups\n  - read:webhooks\n  - write:webhooks\n  - delete:webhooks\n  how_to_obtain: Obtain a client ID and client secret from Myzone, then request an access token from the token URL using the appropriate grant\n    type.\ndocs: https://docs.myzone.org/reference/oauth-20-grant-types.md\n"
source_yaml_url: https://artifacts.apis.io/myzone/authentication/myzone-authentication.yml
summary_line: 1 scheme
tags:
- Fitness
- MotivationTechnology
- Wearables
- Gym Management
- Software-as-a-Service
- Company
---
