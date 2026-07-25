---
api_key_in:
- header
api_specs:
- filename: deliverart-addresses-api-openapi.yml
  format: yaml
  label: Deliverart Addresses API
  slug: deliverart-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-addresses-api-openapi.yml
- filename: deliverart-companies-api-openapi.yml
  format: yaml
  label: Deliverart Companies API
  slug: deliverart-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-companies-api-openapi.yml
- filename: deliverart-customer-addresses-api-openapi.yml
  format: yaml
  label: Deliverart Customer addresses API
  slug: deliverart-customer-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customer-addresses-api-openapi.yml
- filename: deliverart-customer-business-profiles-api-openapi.yml
  format: yaml
  label: Deliverart Customer business profiles API
  slug: deliverart-customer-business-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customer-business-profiles-api-openapi.yml
- filename: deliverart-customers-api-openapi.yml
  format: yaml
  label: Deliverart Customers API
  slug: deliverart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customers-api-openapi.yml
- filename: deliverart-deliveries-api-openapi.yml
  format: yaml
  label: Deliverart Deliveries API
  slug: deliverart-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-deliveries-api-openapi.yml
- filename: deliverart-delivery-fee-api-openapi.yml
  format: yaml
  label: Deliverart Delivery fee API
  slug: deliverart-delivery-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-delivery-fee-api-openapi.yml
- filename: deliverart-me-api-openapi.yml
  format: yaml
  label: Deliverart Me API
  slug: deliverart-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-me-api-openapi.yml
- filename: deliverart-menu-api-openapi.yml
  format: yaml
  label: Deliverart Menu API
  slug: deliverart-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-menu-api-openapi.yml
- filename: deliverart-orders-api-openapi.yml
  format: yaml
  label: Deliverart Orders API
  slug: deliverart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-orders-api-openapi.yml
- filename: deliverart-password-reset-api-openapi.yml
  format: yaml
  label: Deliverart Password reset API
  slug: deliverart-password-reset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-password-reset-api-openapi.yml
- filename: deliverart-points-of-sale-api-openapi.yml
  format: yaml
  label: Deliverart Points of sale API
  slug: deliverart-points-of-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-points-of-sale-api-openapi.yml
- filename: deliverart-registration-api-openapi.yml
  format: yaml
  label: Deliverart Registration API
  slug: deliverart-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-registration-api-openapi.yml
- filename: deliverart-reservation-api-openapi.yml
  format: yaml
  label: Deliverart Reservation API
  slug: deliverart-reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-reservation-api-openapi.yml
- filename: deliverart-take-away-api-openapi.yml
  format: yaml
  label: Deliverart Take away API
  slug: deliverart-take-away-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-take-away-api-openapi.yml
- filename: deliverart-workshifts-api-openapi.yml
  format: yaml
  label: Deliverart Workshifts API
  slug: deliverart-workshifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-workshifts-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deliverart Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Deliverart secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Deliverart
provider_slug: deliverart
scheme_count: 2
schemes:
- description: API key issued by the Deliverart team, sent in the X-Deliverart-ApiKey header.
  in: header
  name: apiKey
  parameter: X-Deliverart-ApiKey
  sources:
  - openapi/deliverart-openapi.yml
  type: apiKey
- description: OAuth2 password grant. Token endpoint is on the auth host.
  flows:
  - flow: password
    scopes: 44
    tokenUrl: https://auth.deliverart.it/oauth
  name: oauth2
  sources:
  - openapi/deliverart-openapi.yml
  type: oauth2
slug: deliverart-authentication
source_filename: deliverart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/deliverart-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Deliverart-ApiKey\n  description: API key issued by the Deliverart team, sent in the X-Deliverart-ApiKey header.\n  sources:\n  - openapi/deliverart-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://auth.deliverart.it/oauth\n    scopes: 44\n  description: OAuth2 password grant. Token endpoint is on the auth host.\n  sources:\n  - openapi/deliverart-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/authentication/deliverart-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
---
