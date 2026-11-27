---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bergsonne-allgaeu-de-availability-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Availability API
  slug: bergsonne-allgaeu-de-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-availability-api-openapi.yml
- filename: bergsonne-allgaeu-de-bookings-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Bookings API
  slug: bergsonne-allgaeu-de-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-bookings-api-openapi.yml
- filename: bergsonne-allgaeu-de-fact-sheet-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Fact Sheet API
  slug: bergsonne-allgaeu-de-fact-sheet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-fact-sheet-api-openapi.yml
- filename: bergsonne-allgaeu-de-hotel-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Hotel API
  slug: bergsonne-allgaeu-de-hotel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-hotel-api-openapi.yml
- filename: bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Hotel Bergsonne Allgäu Booking API
  slug: bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api-openapi.yml
- filename: bergsonne-allgaeu-de-price-quote-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Price Quote API
  slug: bergsonne-allgaeu-de-price-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-price-quote-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hotel Bergsonne Allgäu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotel Bergsonne Allgäu declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hotel Bergsonne Allgäu
provider_slug: bergsonne-allgaeu-de
scheme_count: 1
schemes:
- authorizationUrl: https://bergsonne-allgaeu.de/.well-known/oauth-authorization-server
  flow: authorizationCode
  pkce: true
  scopes:
    booking:read: Read availability and pricing.
    booking:write: Create bookings.
    hotel:read: Read hotel metadata.
  tokenUrl: https://bergsonne-allgaeu.de/.well-known/oauth-authorization-server
  type: oauth2
slug: bergsonne-allgaeu-de-authentication
source_filename: bergsonne-allgaeu-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://bergsonne-allgaeu.de/developers.md\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://bergsonne-allgaeu.de/.well-known/oauth-authorization-server\n    tokenUrl: https://bergsonne-allgaeu.de/.well-known/oauth-authorization-server\n    scopes:\n      hotel:read: Read hotel metadata.\n      booking:read: Read availability and pricing.\n      booking:write: Create bookings.\n"
source_yaml_url: https://artifacts.apis.io/bergsonne-allgaeu-de/authentication/bergsonne-allgaeu-de-authentication.yml
summary_line: 1 scheme
tags:
- Hotels
- Hospitality
- Travel
- Germany
- Allgäu
- Retreat
---
