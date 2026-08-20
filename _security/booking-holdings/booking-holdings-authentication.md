---
api_key_in: []
api_specs:
- filename: booking-holdings-accommodations-api-openapi.yml
  format: yaml
  label: Booking Holdings Accommodations API
  slug: booking-holdings-accommodations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-accommodations-api-openapi.yml
- filename: booking-holdings-attachments-api-openapi.yml
  format: yaml
  label: Booking Holdings Attachments API
  slug: booking-holdings-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-attachments-api-openapi.yml
- filename: booking-holdings-cars-api-openapi.yml
  format: yaml
  label: Booking Holdings Cars API
  slug: booking-holdings-cars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-cars-api-openapi.yml
- filename: booking-holdings-common-languages-api-openapi.yml
  format: yaml
  label: Booking Holdings Common/languages API
  slug: booking-holdings-common-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-common-languages-api-openapi.yml
- filename: booking-holdings-common-locations-api-openapi.yml
  format: yaml
  label: Booking Holdings Common/locations API
  slug: booking-holdings-common-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-common-locations-api-openapi.yml
- filename: booking-holdings-common-payments-api-openapi.yml
  format: yaml
  label: Booking Holdings Common/payments API
  slug: booking-holdings-common-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-common-payments-api-openapi.yml
- filename: booking-holdings-conversations-api-openapi.yml
  format: yaml
  label: Booking Holdings Conversations API
  slug: booking-holdings-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-conversations-api-openapi.yml
- filename: booking-holdings-messages-api-openapi.yml
  format: yaml
  label: Booking Holdings Messages API
  slug: booking-holdings-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-messages-api-openapi.yml
- filename: booking-holdings-orders-api-openapi.yml
  format: yaml
  label: Booking Holdings Orders API
  slug: booking-holdings-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-holdings-orders-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Booking Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booking Holdings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Booking Holdings
provider_slug: booking-holdings
scheme_count: 1
schemes:
- bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/booking-com-demand-api.yaml
  type: http
slug: booking-holdings-authentication
source_filename: booking-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/booking-com-demand-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  sources:\n  - openapi/booking-com-demand-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/authentication/booking-holdings-authentication.yml
summary_line: http · 1 scheme
tags:
- Accommodations
- Airlines
- Car Rentals
- Hospitality
- Hotels
- Restaurant
- Travel
---
