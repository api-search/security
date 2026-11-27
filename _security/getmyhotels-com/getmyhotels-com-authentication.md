---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getmyhotels-com-account-api-openapi.yml
  format: yaml
  label: GetMyHotels Account API
  slug: getmyhotels-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-account-api-openapi.yml
- filename: getmyhotels-com-admin-api-openapi.yml
  format: yaml
  label: GetMyHotels Admin API
  slug: getmyhotels-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-admin-api-openapi.yml
- filename: getmyhotels-com-app-api-openapi.yml
  format: yaml
  label: GetMyHotels App API
  slug: getmyhotels-com-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-app-api-openapi.yml
- filename: getmyhotels-com-bookings-api-openapi.yml
  format: yaml
  label: GetMyHotels Bookings API
  slug: getmyhotels-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-bookings-api-openapi.yml
- filename: getmyhotels-com-chat-api-openapi.yml
  format: yaml
  label: GetMyHotels Chat API
  slug: getmyhotels-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-chat-api-openapi.yml
- filename: getmyhotels-com-consents-api-openapi.yml
  format: yaml
  label: GetMyHotels Consents API
  slug: getmyhotels-com-consents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-consents-api-openapi.yml
- filename: getmyhotels-com-devices-api-openapi.yml
  format: yaml
  label: GetMyHotels Devices API
  slug: getmyhotels-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-devices-api-openapi.yml
- filename: getmyhotels-com-favorites-api-openapi.yml
  format: yaml
  label: GetMyHotels Favorites API
  slug: getmyhotels-com-favorites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-favorites-api-openapi.yml
- filename: getmyhotels-com-flights-api-openapi.yml
  format: yaml
  label: GetMyHotels Flights API
  slug: getmyhotels-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-flights-api-openapi.yml
- filename: getmyhotels-com-hotels-api-openapi.yml
  format: yaml
  label: GetMyHotels Hotels API
  slug: getmyhotels-com-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-hotels-api-openapi.yml
- filename: getmyhotels-com-live-activities-api-openapi.yml
  format: yaml
  label: GetMyHotels Live Activities API
  slug: getmyhotels-com-live-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-live-activities-api-openapi.yml
- filename: getmyhotels-com-notifications-api-openapi.yml
  format: yaml
  label: GetMyHotels Notifications API
  slug: getmyhotels-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-notifications-api-openapi.yml
- filename: getmyhotels-com-payment-methods-api-openapi.yml
  format: yaml
  label: GetMyHotels Payment Methods API
  slug: getmyhotels-com-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-payment-methods-api-openapi.yml
- filename: getmyhotels-com-payments-api-openapi.yml
  format: yaml
  label: GetMyHotels Payments API
  slug: getmyhotels-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-payments-api-openapi.yml
- filename: getmyhotels-com-phone-api-openapi.yml
  format: yaml
  label: GetMyHotels Phone API
  slug: getmyhotels-com-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-phone-api-openapi.yml
- filename: getmyhotels-com-price-watches-api-openapi.yml
  format: yaml
  label: GetMyHotels Price Watches API
  slug: getmyhotels-com-price-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-price-watches-api-openapi.yml
- filename: getmyhotels-com-support-api-openapi.yml
  format: yaml
  label: GetMyHotels Support API
  slug: getmyhotels-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-support-api-openapi.yml
- filename: getmyhotels-com-trips-api-openapi.yml
  format: yaml
  label: GetMyHotels Trips API
  slug: getmyhotels-com-trips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyhotels-com/openapi/getmyhotels-com-trips-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GetMyHotels Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetMyHotels secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GetMyHotels
provider_slug: getmyhotels-com
scheme_count: 1
schemes:
- description: 'Better Auth session token. Obtain it from the native /api/auth/* endpoints (Better Auth bearer plugin — out of scope for this spec, see #922).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/getmyhotels-com-openapi.json
  type: http
slug: getmyhotels-com-authentication
source_filename: getmyhotels-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getmyhotels-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Better Auth session token. Obtain it from the native /api/auth/* endpoints (Better\n    Auth bearer plugin — out of scope for this spec, see #922).'\n  sources:\n  - openapi/getmyhotels-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getmyhotels-com/authentication/getmyhotels-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Travel
- Hotels
- Booking
- Concierge
---
