---
api_key_in:
- header
api_specs:
- filename: tablecheck-availability.yml
  format: yaml
  label: TableCheck Availability API
  slug: tablecheck-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-availability.yml
- filename: tablecheck-web-booking.yml
  format: yaml
  label: TableCheck Web Booking API
  slug: tablecheck-web-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-web-booking.yml
- filename: tablecheck-booking.yml
  format: yaml
  label: TableCheck Booking API
  slug: tablecheck-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-booking.yml
- filename: tablecheck-crm.yml
  format: yaml
  label: TableCheck CRM API
  slug: tablecheck-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-crm.yml
- filename: tablecheck-pos.yml
  format: yaml
  label: TableCheck POS API
  slug: tablecheck-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-pos.yml
- filename: tablecheck-site-controller.yml
  format: yaml
  label: TableCheck Site Controller API
  slug: tablecheck-site-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-site-controller.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tablecheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: TableCheck secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TableCheck
provider_slug: tablecheck
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: AUTHORIZATION
  sources:
  - openapi/tablecheck-availability.yml
  - openapi/tablecheck-booking.yml
  - openapi/tablecheck-pos.yml
  - openapi/tablecheck-site-controller.yml
  - openapi/tablecheck-web-booking.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tablecheck-crm.yml
  type: apiKey
slug: tablecheck-authentication
source_filename: tablecheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tablecheck-availability.yml, openapi/tablecheck-booking.yml, openapi/tablecheck-crm.yml,\n  openapi/tablecheck-pos.yml, openapi/tablecheck-site-controller.yml, openapi/tablecheck-web-booking.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  sources:\n  - openapi/tablecheck-availability.yml\n  - openapi/tablecheck-booking.yml\n  - openapi/tablecheck-pos.yml\n  - openapi/tablecheck-site-controller.yml\n  - openapi/tablecheck-web-booking.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/tablecheck-crm.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/authentication/tablecheck-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Restaurant
- Reservations
- Booking
- Hospitality
- Availability
- Guest CRM
- Point of Sale
- Japan
---
