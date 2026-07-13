---
api_key_in: []
api_specs:
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Search API
  slug: hotel-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Page / Prebook API
  slug: hotel-page-prebook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Order Booking API
  slug: order-booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Content / Static API
  slug: hotel-content-static
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
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
