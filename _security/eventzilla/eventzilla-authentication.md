---
api_key_in:
- header
api_specs:
- filename: eventzilla-attendees-api-openapi.yml
  format: yaml
  label: Eventzilla Attendees API
  slug: eventzilla-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-attendees-api-openapi.yml
- filename: eventzilla-categories-api-openapi.yml
  format: yaml
  label: Eventzilla Categories API
  slug: eventzilla-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-categories-api-openapi.yml
- filename: eventzilla-checkout-api-openapi.yml
  format: yaml
  label: Eventzilla Checkout API
  slug: eventzilla-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-checkout-api-openapi.yml
- filename: eventzilla-events-api-openapi.yml
  format: yaml
  label: Eventzilla Events API
  slug: eventzilla-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-events-api-openapi.yml
- filename: eventzilla-tickets-api-openapi.yml
  format: yaml
  label: Eventzilla Tickets API
  slug: eventzilla-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-tickets-api-openapi.yml
- filename: eventzilla-transactions-api-openapi.yml
  format: yaml
  label: Eventzilla Transactions API
  slug: eventzilla-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-transactions-api-openapi.yml
- filename: eventzilla-users-api-openapi.yml
  format: yaml
  label: Eventzilla Users API
  slug: eventzilla-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/eventzilla-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eventzilla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eventzilla secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eventzilla
provider_slug: eventzilla
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: eventzilla-authentication
source_filename: eventzilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/authentication/eventzilla-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Events
- Ticketing
- Registration
- Attendees
- Event Management
---
