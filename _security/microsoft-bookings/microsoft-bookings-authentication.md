---
api_key_in: []
api_specs:
- filename: microsoft-bookings-appointments-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Appointments API
  slug: microsoft-bookings-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-appointments-api-openapi.yml
- filename: microsoft-bookings-bookingbusinesses-api-openapi.yml
  format: yaml
  label: Microsoft Bookings BookingBusinesses API
  slug: microsoft-bookings-bookingbusinesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-bookingbusinesses-api-openapi.yml
- filename: microsoft-bookings-currencies-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Currencies API
  slug: microsoft-bookings-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-currencies-api-openapi.yml
- filename: microsoft-bookings-customers-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Customers API
  slug: microsoft-bookings-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-customers-api-openapi.yml
- filename: microsoft-bookings-customquestions-api-openapi.yml
  format: yaml
  label: Microsoft Bookings CustomQuestions API
  slug: microsoft-bookings-customquestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-customquestions-api-openapi.yml
- filename: microsoft-bookings-services-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Services API
  slug: microsoft-bookings-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-services-api-openapi.yml
- filename: microsoft-bookings-staffmembers-api-openapi.yml
  format: yaml
  label: Microsoft Bookings StaffMembers API
  slug: microsoft-bookings-staffmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-staffmembers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Bookings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bookings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Bookings
provider_slug: microsoft-bookings
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-bookings-openapi.yml
  type: http
slug: microsoft-bookings-authentication
source_filename: microsoft-bookings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bookings-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-bookings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/authentication/microsoft-bookings-authentication.yml
summary_line: http · 1 scheme
tags:
- Bookings
- Scheduling
- Appointments
- Microsoft Graph
---
