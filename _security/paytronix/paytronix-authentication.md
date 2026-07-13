---
api_key_in: []
api_specs:
- filename: paytronix-server-api-openapi.yml
  format: yaml
  label: Paytronix Server API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-server-api-openapi.yml
- filename: paytronix-online-ordering-api-openapi.yml
  format: yaml
  label: Paytronix Online Ordering API
  slug: online-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytronix/refs/heads/main/openapi/paytronix-online-ordering-api-openapi.yml
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
