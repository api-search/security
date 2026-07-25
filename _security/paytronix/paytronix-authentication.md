---
api_key_in: []
api_specs:
- filename: paytronix-check-api-openapi.yml
  format: yaml
  label: Paytronix Check API
  slug: paytronix-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-check-api-openapi.yml
- filename: paytronix-enrollment-api-openapi.yml
  format: yaml
  label: Paytronix Enrollment API
  slug: paytronix-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-enrollment-api-openapi.yml
- filename: paytronix-gift-api-openapi.yml
  format: yaml
  label: Paytronix Gift API
  slug: paytronix-gift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-gift-api-openapi.yml
- filename: paytronix-guest-api-openapi.yml
  format: yaml
  label: Paytronix Guest API
  slug: paytronix-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-guest-api-openapi.yml
- filename: paytronix-menu-items-api-openapi.yml
  format: yaml
  label: Paytronix Menu Items API
  slug: paytronix-menu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-menu-items-api-openapi.yml
- filename: paytronix-oauth-api-openapi.yml
  format: yaml
  label: Paytronix OAuth API
  slug: paytronix-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-oauth-api-openapi.yml
- filename: paytronix-orders-api-openapi.yml
  format: yaml
  label: Paytronix Orders API
  slug: paytronix-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-orders-api-openapi.yml
- filename: paytronix-payment-api-openapi.yml
  format: yaml
  label: Paytronix Payment API
  slug: paytronix-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-payment-api-openapi.yml
- filename: paytronix-restaurants-api-openapi.yml
  format: yaml
  label: Paytronix Restaurants API
  slug: paytronix-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-restaurants-api-openapi.yml
- filename: paytronix-search-api-openapi.yml
  format: yaml
  label: Paytronix Search API
  slug: paytronix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-search-api-openapi.yml
- filename: paytronix-store-api-openapi.yml
  format: yaml
  label: Paytronix Store API
  slug: paytronix-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-store-api-openapi.yml
- filename: paytronix-transaction-api-openapi.yml
  format: yaml
  label: Paytronix Transaction API
  slug: paytronix-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-transaction-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paytronix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paytronix secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paytronix
provider_slug: paytronix
scheme_count: 2
schemes:
- description: HTTP Basic authentication with the base64-encoded integration identifier and secret (identifier:secret).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/paytronix-server-api-openapi.yml
  type: http
- bearerFormat: OAuth
  description: OAuth bearer token issued by the OAuth Service for guest-scoped operations.
  name: guestBearer
  scheme: bearer
  sources:
  - openapi/paytronix-server-api-openapi.yml
  type: http
slug: paytronix-authentication
source_filename: paytronix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paytronix-server-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with the base64-encoded integration identifier and\n    secret (identifier:secret).\n  sources:\n  - openapi/paytronix-server-api-openapi.yml\n- name: guestBearer\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth\n  description: OAuth bearer token issued by the OAuth Service for guest-scoped operations.\n  sources:\n  - openapi/paytronix-server-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/authentication/paytronix-authentication.yml
summary_line: http · 2 schemes
tags:
- Restaurant
- Loyalty
- Gift Cards
- Online Ordering
- Guest Engagement
- Payments
- Messaging
---
