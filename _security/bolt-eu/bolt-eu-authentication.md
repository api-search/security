---
api_key_in:
- header
api_specs:
- filename: bolt-eu-food-openapi.yml
  format: yaml
  label: Bolt Food API
  slug: bolt-eu-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-food-openapi.yml
- filename: bolt-eu-stores-openapi.yml
  format: yaml
  label: Bolt Stores API
  slug: bolt-eu-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-stores-openapi.yml
- filename: bolt-eu-delivery-openapi.yml
  format: yaml
  label: Bolt Delivery API
  slug: bolt-eu-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-delivery-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bolt Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bolt secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bolt
provider_slug: bolt-eu
scheme_count: 1
schemes:
- description: Partner-gated HMAC request signing. Every request carries the integrator ID in `x-external-integrator-id` plus a `x-server-authorization-hmac-sha256` header containing the base64-encoded HMAC-SHA256 signature of the raw payload, computed with a secret key issued by Bolt. Webhook calls from Bolt to the partner authenticate with Basic auth or a partner-hosted identity server issuing bearer tokens.
  in: header
  name: boltHmacSignature
  parameter: x-external-integrator-id
  sources:
  - openapi/bolt-eu-delivery-openapi.yml
  - openapi/bolt-eu-food-openapi.yml
  - openapi/bolt-eu-stores-openapi.yml
  type: apiKey
slug: bolt-eu-authentication
source_filename: bolt-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bolt-eu-delivery-openapi.yml, openapi/bolt-eu-food-openapi.yml, openapi/bolt-eu-stores-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: boltHmacSignature\n  type: apiKey\n  in: header\n  parameter: x-external-integrator-id\n  description: Partner-gated HMAC request signing. Every request carries the integrator ID in\n    `x-external-integrator-id` plus a `x-server-authorization-hmac-sha256` header containing\n    the base64-encoded HMAC-SHA256 signature of the raw payload, computed with a secret key\n    issued by Bolt. Webhook calls from Bolt to the partner authenticate with Basic auth or a\n    partner-hosted identity server issuing bearer tokens.\n  sources:\n  - openapi/bolt-eu-delivery-openapi.yml\n  - openapi/bolt-eu-food-openapi.yml\n  - openapi/bolt-eu-stores-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/authentication/bolt-eu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ride Booking
- Ride Hailing
- Mobility
- Transportation
- Food Delivery
- Micromobility
- Delivery
- Super App
---
