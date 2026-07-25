---
api_key_in: []
api_specs:
- filename: autopay-accounting-api-openapi.yml
  format: yaml
  label: Autopay Accounting API
  slug: autopay-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-accounting-api-openapi.yml
- filename: autopay-booking-api-openapi.yml
  format: yaml
  label: Autopay Booking API
  slug: autopay-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-booking-api-openapi.yml
- filename: autopay-customer-club-api-openapi.yml
  format: yaml
  label: Autopay Customer Club API
  slug: autopay-customer-club-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-customer-club-api-openapi.yml
- filename: autopay-fleet-api-openapi.yml
  format: yaml
  label: Autopay Fleet API
  slug: autopay-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-fleet-api-openapi.yml
- filename: autopay-parking-api-openapi.yml
  format: yaml
  label: Autopay Parking API
  slug: autopay-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-parking-api-openapi.yml
- filename: autopay-payment-api-openapi.yml
  format: yaml
  label: Autopay Payment API
  slug: autopay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-payment-api-openapi.yml
- filename: autopay-permit-api-openapi.yml
  format: yaml
  label: Autopay Permit API
  slug: autopay-permit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-permit-api-openapi.yml
- filename: autopay-statistics-api-openapi.yml
  format: yaml
  label: Autopay Statistics API
  slug: autopay-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-statistics-api-openapi.yml
- filename: autopay-status-api-openapi.yml
  format: yaml
  label: Autopay Status API
  slug: autopay-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-status-api-openapi.yml
- filename: autopay-vehicle-api-openapi.yml
  format: yaml
  label: Autopay Vehicle API
  slug: autopay-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-vehicle-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Autopay Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Autopay secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Autopay
provider_slug: autopay
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow. Tokens are minted from the Auth0 token endpoint and used as Bearer tokens with `audience` set to `https://api.autopay.io`. Some endpoints require specific scopes such as `permit_booking`, `customer_club`, or `zone_status`.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api-auth.autopay.io/oauth/token
  name: OAuth2
  sources:
  - openapi/autopay-openapi.yml
  type: oauth2
slug: autopay-authentication
source_filename: autopay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autopay-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-auth.autopay.io/oauth/token\n    scopes: 3\n  description: OAuth 2.0 Client Credentials flow. Tokens are minted from the Auth0 token endpoint\n    and used as Bearer tokens with `audience` set to `https://api.autopay.io`. Some endpoints\n    require specific scopes such as `permit_booking`, `customer_club`, or `zone_status`.\n  sources:\n  - openapi/autopay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/authentication/autopay-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Parking
- Parking Payments
- Fleet Management
- Permits
- Parking Operators
- Norway
---
