---
api_key_in:
- header
api_specs:
- filename: maersk-track-and-trace-api-openapi.yml
  format: yaml
  label: Maersk Track and Trace API
  slug: maersk-track-and-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-track-and-trace-api-openapi.yml
- filename: maersk-ocean-booking-api-openapi.yml
  format: yaml
  label: Maersk Ocean Booking API
  slug: maersk-ocean-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-ocean-booking-api-openapi.yml
- filename: maersk-schedules-api-openapi.yml
  format: yaml
  label: Maersk Schedules API
  slug: maersk-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-schedules-api-openapi.yml
- filename: maersk-product-offers-api-openapi.yml
  format: yaml
  label: Maersk Product Offers API
  slug: maersk-product-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-product-offers-api-openapi.yml
- filename: maersk-bill-of-lading-api-openapi.yml
  format: yaml
  label: Maersk Bill of Lading API
  slug: maersk-bill-of-lading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-bill-of-lading-api-openapi.yml
- filename: maersk-vgm-api-openapi.yml
  format: yaml
  label: Maersk Verified Gross Mass API
  slug: maersk-vgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-vgm-api-openapi.yml
- filename: maersk-demurrage-detention-api-openapi.yml
  format: yaml
  label: Maersk Import Demurrage and Detention API
  slug: maersk-demurrage-detention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-demurrage-detention-api-openapi.yml
- filename: maersk-air-booking-api-openapi.yml
  format: yaml
  label: Maersk Air Booking API
  slug: maersk-air-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-air-booking-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Maersk Line Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Maersk secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Maersk
provider_slug: maersk-line
scheme_count: 3
schemes:
- in: header
  name: ConsumerKey
  parameter: Consumer-Key
  sources:
  - openapi/maersk-air-booking-api-openapi.yml
  - openapi/maersk-bill-of-lading-api-openapi.yml
  - openapi/maersk-demurrage-detention-api-openapi.yml
  - openapi/maersk-ocean-booking-api-openapi.yml
  - openapi/maersk-product-offers-api-openapi.yml
  - openapi/maersk-schedules-api-openapi.yml
  - openapi/maersk-track-and-trace-api-openapi.yml
  - openapi/maersk-vgm-api-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token
  name: OAuth2
  sources:
  - openapi/maersk-bill-of-lading-api-openapi.yml
  - openapi/maersk-ocean-booking-api-openapi.yml
  - openapi/maersk-track-and-trace-api-openapi.yml
  - openapi/maersk-vgm-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: ForgeRockJWT
  scheme: bearer
  sources:
  - openapi/maersk-product-offers-api-openapi.yml
  type: http
slug: maersk-line-authentication
source_filename: maersk-line-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maersk-air-booking-api-openapi.yml, openapi/maersk-bill-of-lading-api-openapi.yml,\n  openapi/maersk-demurrage-detention-api-openapi.yml, openapi/maersk-ocean-booking-api-openapi.yml,\n  openapi/maersk-product-offers-api-openapi.yml, openapi/maersk-schedules-api-openapi.yml, openapi/maersk-track-and-trace-api-openapi.yml,\n  openapi/maersk-vgm-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ConsumerKey\n  type: apiKey\n  in: header\n  parameter: Consumer-Key\n  sources:\n  - openapi/maersk-air-booking-api-openapi.yml\n  - openapi/maersk-bill-of-lading-api-openapi.yml\n  - openapi/maersk-demurrage-detention-api-openapi.yml\n  - openapi/maersk-ocean-booking-api-openapi.yml\n  - openapi/maersk-product-offers-api-openapi.yml\n  - openapi/maersk-schedules-api-openapi.yml\n  - openapi/maersk-track-and-trace-api-openapi.yml\n\
  \  - openapi/maersk-vgm-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token\n    scopes: 1\n  sources:\n  - openapi/maersk-bill-of-lading-api-openapi.yml\n  - openapi/maersk-ocean-booking-api-openapi.yml\n  - openapi/maersk-track-and-trace-api-openapi.yml\n  - openapi/maersk-vgm-api-openapi.yml\n- name: ForgeRockJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/maersk-product-offers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/authentication/maersk-line-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Shipping
- Logistics
- Container Shipping
- Ocean Freight
- Air Freight
- Supply Chain
- DCSA
- Maritime
---
