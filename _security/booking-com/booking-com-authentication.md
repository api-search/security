---
anonymous_access: false
api_key_in: []
api_specs:
- filename: booking-com-demand-api-3-2-openapi.yml
  format: yaml
  label: Booking.com Demand API
  slug: booking-com-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-demand-api-3-2-openapi.yml
- filename: booking-com-connect-api-openapi.yml
  format: yaml
  label: Booking.com Connect API
  slug: booking-com-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connect-api-openapi.yml
- filename: booking-com-status-api-openapi.yml
  format: yaml
  label: Booking.com Status API
  slug: booking-com-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-status-api-openapi.yml
- filename: booking-com-charges-api-openapi.yml
  format: yaml
  label: Booking.com Charges API
  slug: booking-com-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-charges-api-openapi.yml
- filename: booking-com-contacts-api-openapi.yml
  format: yaml
  label: Booking.com Contacts API
  slug: booking-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contacts-api-openapi.yml
- filename: booking-com-contracting-api-openapi.yml
  format: yaml
  label: Booking.com Contracting API
  slug: booking-com-contracting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contracting-api-openapi.yml
- filename: booking-com-facilities-api-openapi.yml
  format: yaml
  label: Booking.com Facilities API
  slug: booking-com-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-facilities-api-openapi.yml
- filename: booking-com-historical-reservations-api-openapi.yml
  format: yaml
  label: Booking.com Historical Reservations API
  slug: booking-com-historical-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-historical-reservations-api-openapi.yml
- filename: booking-com-payments-api-openapi.yml
  format: yaml
  label: Booking.com Payments API
  slug: booking-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-api-openapi.yml
- filename: booking-com-payments-by-booking-onboarding-api-openapi.yml
  format: yaml
  label: Booking.com Payments by Booking Onboarding API
  slug: booking-com-payments-by-booking-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml
- filename: booking-com-property-api-openapi.yml
  format: yaml
  label: Booking.com Property API
  slug: booking-com-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-api-openapi.yml
- filename: booking-com-property-health-api-openapi.yml
  format: yaml
  label: Booking.com Property Health API
  slug: booking-com-property-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-health-api-openapi.yml
- filename: booking-com-reconciliation-api-openapi.yml
  format: yaml
  label: Booking.com Reconciliation API
  slug: booking-com-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-reconciliation-api-openapi.yml
- filename: booking-com-rooms-api-openapi.yml
  format: yaml
  label: Booking.com Rooms API
  slug: booking-com-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-rooms-api-openapi.yml
- filename: booking-com-valueadds-api-openapi.yml
  format: yaml
  label: Booking.com Value Adds Catalog API
  slug: booking-com-valueadds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-valueadds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Booking Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booking.com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Booking.com
provider_slug: booking-com
scheme_count: 1
schemes:
- applies_to:
  - Booking.com Demand API (3.1, 3.2, 3.2-Beta)
  - Booking.com Connect API
  - Historical Reservations API
  - Payments API
  - Payments by Booking Onboarding API
  - Property Health API
  - Reconciliation API
  bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/booking-com-demand-api-3-2-openapi.yml
  - openapi/booking-com-demand-api-3-1-openapi.yml
  - openapi/booking-com-demand-api-3-2-beta-openapi.yml
  - openapi/booking-com-connect-api-openapi.yml
  - openapi/booking-com-historical-reservations-api-openapi.yml
  - openapi/booking-com-payments-api-openapi.yml
  - openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml
  - openapi/booking-com-property-health-api-openapi.yml
  - openapi/booking-com-reconciliation-api-openapi.yml
  type: http
slug: booking-com-authentication
source_filename: booking-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://developers.booking.com/demand/docs/development-guide/authentication and\n  https://developers.booking.com/connectivity/docs/authentication, reconciled against the\n  securitySchemes declared in the 20 OpenAPI descriptions in openapi/.\ndocs:\n- https://developers.booking.com/demand/docs/development-guide/authentication\n- https://developers.booking.com/connectivity/docs/authentication\n- https://developers.booking.com/connectivity/docs/token-based-authentication\nsummary:\n  types:\n  - http\n  styles:\n  - bearer token + affiliate header (Demand API)\n  - JWT from machine-account credentials (Connectivity APIs)\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect anywhere. Both programmes are bearer-token schemes issued through a\n    partner portal, so there is no scope model to record and no authorization-server metadata to fetch.\nschemes:\n- name:\
  \ BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  applies_to:\n  - Booking.com Demand API (3.1, 3.2, 3.2-Beta)\n  - Booking.com Connect API\n  - Historical Reservations API\n  - Payments API\n  - Payments by Booking Onboarding API\n  - Property Health API\n  - Reconciliation API\n  sources:\n  - openapi/booking-com-demand-api-3-2-openapi.yml\n  - openapi/booking-com-demand-api-3-1-openapi.yml\n  - openapi/booking-com-demand-api-3-2-beta-openapi.yml\n  - openapi/booking-com-connect-api-openapi.yml\n  - openapi/booking-com-historical-reservations-api-openapi.yml\n  - openapi/booking-com-payments-api-openapi.yml\n  - openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml\n  - openapi/booking-com-property-health-api-openapi.yml\n  - openapi/booking-com-reconciliation-api-openapi.yml\nprogrammes:\n- name: Demand API (affiliate partners)\n  credential_pair: true\n  headers:\n  - name: Authorization\n    value: 'Bearer <key>'\n    note: The API key token generated\
  \ for the API user.\n  - name: X-Affiliate-Id\n    value: '<aid>'\n    note: >-\n      REQUIRED alongside the bearer token on every request, production and sandbox alike. An API user is\n      the pair (partner ID, affiliate ID); the spec's single BearerAuth scheme understates this - the\n      affiliate header is not modelled as a securityScheme.\n  key_issuance: Affiliate Partner Centre (partner login), self-service key generation\n  key_rotation: Booking.com recommends generating a new API key every 12 months; keys can be replaced or revoked earlier.\n  transport: HTTPS only; requests over HTTP are rejected.\n  sandbox_credentials: same as production - no sandbox-specific keys\n  docs: https://developers.booking.com/demand/docs/development-guide/authentication\n- name: Connectivity APIs (supply / channel-manager partners)\n  credential_pair: false\n  scheme: JSON Web Token in the Authorization header\n  token_lifetime: 1 hour; a new token is generated from machine-account credentials\
  \ each hour\n  token_revocable: true\n  issuance: Machine accounts created in the Connectivity Portal (https://connect.booking.com), scoped at property level\n  superseded_scheme:\n    name: Credential-based authentication\n    deprecated: '2025-06-30'\n    sunset: '2025-12-31'\n    note: >-\n      The older per-request machine-account credential scheme was sunset on 31 December 2025 under\n      Booking.com's published deprecation policy. Token-based authentication is now the only supported\n      Connectivity scheme.\n  docs: https://developers.booking.com/connectivity/docs/token-based-authentication\ngaps:\n- id: affiliate-header-not-in-spec\n  detail: >-\n    X-Affiliate-Id is mandatory per the docs but is absent from the Demand API securitySchemes. An agent\n    reading only the OpenAPI would build a request that always 401s.\n- id: specs-without-security\n  detail: >-\n    Nine of the twenty published specs (charges, contacts, contracting, facilities x2, property, rooms x3,\n   \
  \ valueadds, status) declare no securitySchemes and no security requirement at all, even though the\n    Connectivity docs state every request carries a JWT. The contracting-api description states the JWT\n    requirement in prose inside info.description rather than declaring it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/authentication/booking-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Hospitality
- Accommodation
- Booking
- Car Rental
- Payments
- Connectivity
- Marketplace
- OTA
- Attractions
- A2A
- Hotels
---
