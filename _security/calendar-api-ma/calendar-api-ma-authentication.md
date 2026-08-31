---
api_key_in:
- cookie
- header
api_specs:
- filename: calendar-api-ma-business-days-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Business Days API
  slug: calendar-api-ma-business-days-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-business-days-api-openapi.yml
- filename: calendar-api-ma-holidays-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Holidays API
  slug: calendar-api-ma-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-holidays-api-openapi.yml
- filename: calendar-api-ma-misc-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Misc API
  slug: calendar-api-ma-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-misc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Calendar Api Ma Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python
provider_slug: calendar-api-ma
scheme_count: 2
schemes:
- description: API Key authentication and authorization.
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/calendar-api-ma-calendar-api-openapi.yml
  type: apiKey
- description: Session cookie authentication.
  in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - openapi/calendar-api-ma-calendar-api-openapi.yml
  type: apiKey
slug: calendar-api-ma-authentication
source_filename: calendar-api-ma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: derived\nsource: openapi/calendar-api-ma-calendar-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API Key authentication and authorization.\n  sources:\n  - openapi/calendar-api-ma-calendar-api-openapi.yml\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Session cookie authentication.\n  sources:\n  - openapi/calendar-api-ma-calendar-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/authentication/calendar-api-ma-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- holidays
- morocco
- Calendar
- business-days
- date-utilities
- data-engineering
- ETL
- python-sdk
- Localization
- reference-data
- public-holidays
- scheduling
---
