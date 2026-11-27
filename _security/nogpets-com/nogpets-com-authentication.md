---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nogpets-com-account-api-openapi.yml
  format: yaml
  label: NogPets Account API
  slug: nogpets-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-account-api-openapi.yml
- filename: nogpets-com-booking-api-openapi.yml
  format: yaml
  label: NogPets Booking API
  slug: nogpets-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-booking-api-openapi.yml
- filename: nogpets-com-business-api-openapi.yml
  format: yaml
  label: NogPets Business API
  slug: nogpets-com-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-business-api-openapi.yml
- filename: nogpets-com-directory-api-openapi.yml
  format: yaml
  label: NogPets Directory API
  slug: nogpets-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-directory-api-openapi.yml
- filename: nogpets-com-run-api-openapi.yml
  format: yaml
  label: NogPets Run API
  slug: nogpets-com-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-run-api-openapi.yml
- filename: nogpets-com-services-api-openapi.yml
  format: yaml
  label: NogPets Services API
  slug: nogpets-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-services-api-openapi.yml
- filename: nogpets-com-shop-api-openapi.yml
  format: yaml
  label: NogPets Shop API
  slug: nogpets-com-shop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-shop-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NogPets Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NogPets secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NogPets
provider_slug: nogpets-com
scheme_count: 2
schemes:
- description: OAuth 2.1, authorization code with PKCE (S256), public clients. Register with `POST /oauth/register` (RFC 7591). Access tokens last an hour; refresh tokens rotate.
  flows:
  - authorizationUrl: https://api.nogpets.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.nogpets.com/oauth/token
  name: oauth2
  sources:
  - openapi/nogpets-com-openapi.json
  type: oauth2
- bearerFormat: npk_…
  description: A personal API key from the NogPets app (Profile → Connect an AI assistant). It carries the scopes chosen when it was made.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/nogpets-com-openapi.json
  type: http
slug: nogpets-com-authentication
source_filename: nogpets-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nogpets-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.nogpets.com/oauth/authorize\n    tokenUrl: https://api.nogpets.com/oauth/token\n    scopes: 8\n  description: OAuth 2.1, authorization code with PKCE (S256), public clients. Register with\n    `POST /oauth/register` (RFC 7591). Access tokens last an hour; refresh tokens rotate.\n  sources:\n  - openapi/nogpets-com-openapi.json\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: npk_…\n  description: A personal API key from the NogPets app (Profile → Connect an AI assistant).\n    It carries the scopes chosen when it was made.\n  sources:\n  - openapi/nogpets-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nogpets-com/authentication/nogpets-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Grooming
- Dog Walks
- Pet Sitting
- Pet Services
- WhatsApp Booking
- South Africa
---
