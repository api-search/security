---
api_key_in: []
api_specs:
- filename: ratehawk-booking-api-openapi.yml
  format: yaml
  label: RateHawk Booking API
  slug: ratehawk-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-booking-api-openapi.yml
- filename: ratehawk-cancellation-api-openapi.yml
  format: yaml
  label: RateHawk Cancellation API
  slug: ratehawk-cancellation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-cancellation-api-openapi.yml
- filename: ratehawk-hotel-content-api-openapi.yml
  format: yaml
  label: RateHawk Hotel Content API
  slug: ratehawk-hotel-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-hotel-content-api-openapi.yml
- filename: ratehawk-hotel-search-api-openapi.yml
  format: yaml
  label: RateHawk Hotel Search API
  slug: ratehawk-hotel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-hotel-search-api-openapi.yml
- filename: ratehawk-orders-api-openapi.yml
  format: yaml
  label: RateHawk Orders API
  slug: ratehawk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-orders-api-openapi.yml
- filename: ratehawk-prebook-api-openapi.yml
  format: yaml
  label: RateHawk Prebook API
  slug: ratehawk-prebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-prebook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ratehawk Authentication
name_suffix: Authentication
oauth_flows: []
overview: RateHawk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RateHawk
provider_slug: ratehawk
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The username is the API key id and the password is the API key (uuid). Both are issued per contract for the test (sandbox) and production environments.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ratehawk-openapi.yml
  type: http
slug: ratehawk-authentication
source_filename: ratehawk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ratehawk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. The username is the API key id and the password is\n    the API key (uuid). Both are issued per contract for the test (sandbox) and production environments.\n  sources:\n  - openapi/ratehawk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/authentication/ratehawk-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Hotels
- Booking
- B2B
- Reservations
---
