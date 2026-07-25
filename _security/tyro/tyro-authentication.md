---
api_key_in: []
api_specs:
- filename: tyro-connect-pay.yml
  format: yaml
  label: Tyro Connect Pay API
  slug: tyro-connect-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-pay.yml
- filename: tyro-pos-pay-terminal.yml
  format: yaml
  label: Tyro Pay Terminal API
  slug: tyro-pos-pay-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-pos-pay-terminal.yml
- filename: tyro-pos-embedded-payments.yml
  format: yaml
  label: Tyro Embedded Payments API
  slug: tyro-pos-embedded-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-pos-embedded-payments.yml
- filename: tyro-connect-booking.yml
  format: yaml
  label: Tyro Connect Booking API
  slug: tyro-connect-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-booking.yml
- filename: tyro-connect-ordering.yml
  format: yaml
  label: Tyro Connect Ordering API
  slug: tyro-connect-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-ordering.yml
- filename: tyro-connect-menu.yml
  format: yaml
  label: Tyro Connect Menu API
  slug: tyro-connect-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-menu.yml
- filename: tyro-connect-tables.yml
  format: yaml
  label: Tyro Connect Tables Management API
  slug: tyro-connect-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-tables.yml
- filename: tyro-connect-sales.yml
  format: yaml
  label: Tyro Connect Sales Data API
  slug: tyro-connect-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-sales.yml
- filename: tyro-connect-reporting.yml
  format: yaml
  label: Tyro Connect Reporting API
  slug: tyro-connect-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-reporting.yml
- filename: tyro-connect-loyalty.yml
  format: yaml
  label: Tyro Connect Loyalty Data API
  slug: tyro-connect-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-loyalty.yml
- filename: tyro-connect-refunds.yml
  format: yaml
  label: Tyro Connect Refunds API
  slug: tyro-connect-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-refunds.yml
- filename: tyro-connect-locations.yml
  format: yaml
  label: Tyro Connect Location API
  slug: tyro-connect-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-locations.yml
- filename: tyro-connect-referrals.yml
  format: yaml
  label: Tyro Connect Referrals API
  slug: tyro-connect-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/openapi/tyro-connect-referrals.yml
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tyro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tyro Payments secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tyro Payments
provider_slug: tyro
scheme_count: 1
schemes:
- name: JWT
  openIdConnectUrl: https://auth.connect.tyro.com/.well-known/openid-configuration
  sources:
  - openapi/tyro-connect-booking.yml
  - openapi/tyro-connect-locations.yml
  - openapi/tyro-connect-loyalty.yml
  - openapi/tyro-connect-menu.yml
  - openapi/tyro-connect-ordering.yml
  - openapi/tyro-connect-pay.yml
  - openapi/tyro-connect-reporting.yml
  - openapi/tyro-connect-sales.yml
  - openapi/tyro-connect-tables.yml
  - openapi/tyro-pos-embedded-payments.yml
  - openapi/tyro-pos-pay-terminal.yml
  type: openIdConnect
slug: tyro-authentication
source_filename: tyro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\ndocs: https://docs.connect.tyro.com/app/authentication\nflow: OAuth 2.0 Client Credentials (partner requests client_id/client_secret from Tyro)\ntoken:\n  type: JWT bearer (Authorization header)\n  token_endpoint: https://auth.connect.tyro.com/oauth/token\n  ttl_hours: 12\n  token_type: Bearer\n  authz_server_rate_limit: max 12 token requests per 11-hour window (cache tokens)\n  identity_provider: Auth0\nspecial_headers:\n  - Pay-Secret (client-side secret to drive a Pay Request from Tyro.js / hosted pay sheet)\nsource: openapi/tyro-connect-booking.yml, openapi/tyro-connect-locations.yml, openapi/tyro-connect-loyalty.yml,\n  openapi/tyro-connect-menu.yml, openapi/tyro-connect-ordering.yml, openapi/tyro-connect-pay.yml,\n  openapi/tyro-connect-reporting.yml, openapi/tyro-connect-sales.yml, openapi/tyro-connect-tables.yml,\n  openapi/tyro-pos-embedded-payments.yml, openapi/tyro-pos-pay-terminal.yml\nsummary:\n  types:\n  - openIdConnect\n\
  schemes:\n- name: JWT\n  type: openIdConnect\n  openIdConnectUrl: https://auth.connect.tyro.com/.well-known/openid-configuration\n  sources:\n  - openapi/tyro-connect-booking.yml\n  - openapi/tyro-connect-locations.yml\n  - openapi/tyro-connect-loyalty.yml\n  - openapi/tyro-connect-menu.yml\n  - openapi/tyro-connect-ordering.yml\n  - openapi/tyro-connect-pay.yml\n  - openapi/tyro-connect-reporting.yml\n  - openapi/tyro-connect-sales.yml\n  - openapi/tyro-connect-tables.yml\n  - openapi/tyro-pos-embedded-payments.yml\n  - openapi/tyro-pos-pay-terminal.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyro/refs/heads/main/authentication/tyro-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Payments
- Australia
- Merchant Acquiring
- Payment Gateway
- In-Person Payments
- EFTPOS
- Point of Sale
- Online Payments
- Tap to Pay
---
