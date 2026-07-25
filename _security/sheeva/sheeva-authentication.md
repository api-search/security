---
api_key_in:
- header
api_specs:
- filename: sheeva-authentication-api-openapi.yml
  format: yaml
  label: Sheeva Authentication API
  slug: sheeva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-authentication-api-openapi.yml
- filename: sheeva-credit-cards-api-openapi.yml
  format: yaml
  label: Sheeva Credit Cards API
  slug: sheeva-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-credit-cards-api-openapi.yml
- filename: sheeva-driver-alerts-api-openapi.yml
  format: yaml
  label: Sheeva Driver Alerts API
  slug: sheeva-driver-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-driver-alerts-api-openapi.yml
- filename: sheeva-driver-api-openapi.yml
  format: yaml
  label: Sheeva Driver API
  slug: sheeva-driver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-driver-api-openapi.yml
- filename: sheeva-feedback-api-openapi.yml
  format: yaml
  label: Sheeva Feedback API
  slug: sheeva-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-feedback-api-openapi.yml
- filename: sheeva-loyalty-api-openapi.yml
  format: yaml
  label: Sheeva Loyalty API
  slug: sheeva-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-loyalty-api-openapi.yml
- filename: sheeva-parking-api-openapi.yml
  format: yaml
  label: Sheeva Parking API
  slug: sheeva-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-parking-api-openapi.yml
- filename: sheeva-payments-api-openapi.yml
  format: yaml
  label: Sheeva Payments API
  slug: sheeva-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-payments-api-openapi.yml
- filename: sheeva-service-hubs-points-of-interest-api-openapi.yml
  format: yaml
  label: Sheeva Service Hubs (Points Of Interest) API
  slug: sheeva-service-hubs-points-of-interest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-service-hubs-points-of-interest-api-openapi.yml
- filename: sheeva-session-api-openapi.yml
  format: yaml
  label: Sheeva Session API
  slug: sheeva-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-session-api-openapi.yml
- filename: sheeva-transactions-api-openapi.yml
  format: yaml
  label: Sheeva Transactions API
  slug: sheeva-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-transactions-api-openapi.yml
- filename: sheeva-upi-api-openapi.yml
  format: yaml
  label: Sheeva UPI API
  slug: sheeva-upi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-upi-api-openapi.yml
- filename: sheeva-vehicle-api-openapi.yml
  format: yaml
  label: Sheeva Vehicle API
  slug: sheeva-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-vehicle-api-openapi.yml
- filename: sheeva-vehicle-events-api-openapi.yml
  format: yaml
  label: Sheeva Vehicle Events API
  slug: sheeva-vehicle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-vehicle-events-api-openapi.yml
- filename: sheeva-webhooks-api-openapi.yml
  format: yaml
  label: Sheeva Webhooks API
  slug: sheeva-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sheeva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sheeva secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sheeva
provider_slug: sheeva
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Access token obtained from GET /v2/auth (exchange client-id/client-secret), sent in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sheeva-openapi.yml
  type: http
- description: client-id + client-secret headers on GET /v2/auth to obtain an access token.
  in: header
  name: clientCredentials
  parameter: client-id
  sources:
  - openapi/sheeva-openapi.yml
  type: apiKey
slug: sheeva-authentication
source_filename: sheeva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sheeva-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token obtained from GET /v2/auth (exchange client-id/client-secret), sent\n    in the Authorization header.\n  sources:\n  - openapi/sheeva-openapi.yml\n- name: clientCredentials\n  type: apiKey\n  in: header\n  parameter: client-id\n  description: client-id + client-secret headers on GET /v2/auth to obtain an access token.\n  sources:\n  - openapi/sheeva-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/authentication/sheeva-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Connected Vehicles
- Automotive
- Payments
- Fintech
- In-Vehicle Payments
- EV Charging
- Parking
- Location Intelligence
- Mobility
---
