---
api_key_in: []
api_specs:
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offer Requests API
  slug: duffel-offer-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offers API
  slug: duffel-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Orders API
  slug: duffel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Seat Maps API
  slug: duffel-seat-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Changes API
  slug: duffel-order-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Cancellations API
  slug: duffel-order-cancellations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Payments API
  slug: duffel-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Stays API
  slug: duffel-stays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Webhooks API
  slug: duffel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Duffel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duffel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duffel
provider_slug: duffel
scheme_count: 1
schemes:
- description: 'Authenticate with your Duffel access token as a Bearer token in the Authorization header (Authorization: Bearer [example key]).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/duffel-openapi.yml
  type: http
slug: duffel-authentication
source_filename: duffel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duffel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with your Duffel access token as a Bearer token in the Authorization\n    header (Authorization: Bearer [example key]).'\n  sources:\n  - openapi/duffel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/authentication/duffel-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Flights
- Hotels
- Booking
- Payments
---
