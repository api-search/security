---
api_key_in:
- header
api_specs:
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Events API
  slug: brushfire-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Attendees API
  slug: brushfire-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Orders API
  slug: brushfire-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Cart & Checkout API
  slug: brushfire-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Sessions & Check-In API
  slug: brushfire-sessions-checkin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Groups API
  slug: brushfire-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Promotions & Access Codes API
  slug: brushfire-promotions-accesscodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Webhooks (Hooks) API
  slug: brushfire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brushfire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brushfire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brushfire
provider_slug: brushfire
scheme_count: 1
schemes:
- description: The App Key you received from https://developer.brushfire.com/key
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/brushfire-openapi.json
  type: apiKey
slug: brushfire-authentication
source_filename: brushfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brushfire-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The App Key you received from https://developer.brushfire.com/key\n  sources:\n  - openapi/brushfire-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/authentication/brushfire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Ticketing
- Registration
- Events
- Ticketing
- Check-In
- Churches
- Payments
---
