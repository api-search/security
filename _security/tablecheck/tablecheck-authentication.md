---
api_key_in:
- header
api_specs:
- filename: tablecheck-availability-api-openapi.yml
  format: yaml
  label: TableCheck availability API
  slug: tablecheck-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-availability-api-openapi.yml
- filename: tablecheck-blockages-api-openapi.yml
  format: yaml
  label: TableCheck blockages API
  slug: tablecheck-blockages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-blockages-api-openapi.yml
- filename: tablecheck-calendar-api-openapi.yml
  format: yaml
  label: TableCheck calendar API
  slug: tablecheck-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-calendar-api-openapi.yml
- filename: tablecheck-customers-api-openapi.yml
  format: yaml
  label: TableCheck customers API
  slug: tablecheck-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-customers-api-openapi.yml
- filename: tablecheck-franchises-api-openapi.yml
  format: yaml
  label: TableCheck franchises API
  slug: tablecheck-franchises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-franchises-api-openapi.yml
- filename: tablecheck-membership-programs-api-openapi.yml
  format: yaml
  label: TableCheck membership_programs API
  slug: tablecheck-membership-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-membership-programs-api-openapi.yml
- filename: tablecheck-memberships-api-openapi.yml
  format: yaml
  label: TableCheck memberships API
  slug: tablecheck-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-memberships-api-openapi.yml
- filename: tablecheck-pos-journals-api-openapi.yml
  format: yaml
  label: TableCheck pos_journals API
  slug: tablecheck-pos-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-pos-journals-api-openapi.yml
- filename: tablecheck-reservation-flags-api-openapi.yml
  format: yaml
  label: TableCheck reservation_flags API
  slug: tablecheck-reservation-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-reservation-flags-api-openapi.yml
- filename: tablecheck-reservations-api-openapi.yml
  format: yaml
  label: TableCheck reservations API
  slug: tablecheck-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-reservations-api-openapi.yml
- filename: tablecheck-shops-api-openapi.yml
  format: yaml
  label: TableCheck shops API
  slug: tablecheck-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-shops-api-openapi.yml
- filename: tablecheck-table-status-api-openapi.yml
  format: yaml
  label: TableCheck table_status API
  slug: tablecheck-table-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-table-status-api-openapi.yml
- filename: tablecheck-tables-api-openapi.yml
  format: yaml
  label: TableCheck tables API
  slug: tablecheck-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-tables-api-openapi.yml
- filename: tablecheck-timetable-api-openapi.yml
  format: yaml
  label: TableCheck timetable API
  slug: tablecheck-timetable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-timetable-api-openapi.yml
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
