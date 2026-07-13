---
api_key_in:
- header
api_specs:
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Forms and Inventory API
  slug: ticketspice-forms-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Orders and Registrants API
  slug: ticketspice-orders-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Tickets API
  slug: ticketspice-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Transactions and Customers API
  slug: ticketspice-transactions-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Coupons API
  slug: ticketspice-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Webhooks API
  slug: ticketspice-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ticketspice Authentication
name_suffix: Authentication
oauth_flows: []
overview: TicketSpice secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TicketSpice
provider_slug: ticketspice
scheme_count: 1
schemes:
- description: Account API key generated from the TicketSpice/Webconnex dashboard.
  in: header
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/ticketspice-openapi.yml
  type: apiKey
slug: ticketspice-authentication
source_filename: ticketspice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ticketspice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Account API key generated from the TicketSpice/Webconnex dashboard.\n  sources:\n  - openapi/ticketspice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/authentication/ticketspice-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Ticketing
- Ticketing
- Events
- Registration
- Payments
- Webconnex
---
