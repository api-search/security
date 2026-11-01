---
anonymous_access: false
api_key_in: []
api_specs:
- filename: addevent-calendar-subscribers-api-openapi.yml
  format: yaml
  label: AddEvent Calendar subscribers API
  slug: addevent-calendar-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendar-subscribers-api-openapi.yml
- filename: addevent-calendars-api-openapi.yml
  format: yaml
  label: AddEvent Calendars API
  slug: addevent-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendars-api-openapi.yml
- filename: addevent-events-api-openapi.yml
  format: yaml
  label: AddEvent Events API
  slug: addevent-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-events-api-openapi.yml
- filename: addevent-rsvp-attendees-api-openapi.yml
  format: yaml
  label: AddEvent RSVP attendees API
  slug: addevent-rsvp-attendees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-rsvp-attendees-api-openapi.yml
- filename: addevent-templates-api-openapi.yml
  format: yaml
  label: AddEvent Templates API
  slug: addevent-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-templates-api-openapi.yml
- filename: addevent-timezones-api-openapi.yml
  format: yaml
  label: AddEvent Timezones API
  slug: addevent-timezones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-timezones-api-openapi.yml
auth_types: []
description: 'Authentication to the API is performed with HTTP Bearer Authentication. Provide your API key in the `Authorization` header when making a request, as follows:'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Addevent Authentication
name_suffix: Authentication
oauth_flows: []
overview: AddEvent declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AddEvent
provider_slug: addevent
scheme_count: 1
schemes:
- evidence: 'Authentication to the API is performed with HTTP Bearer Authentication. Provide your API key in the `Authorization` header when making a request, as follows:'
  header: Authorization
  how_to_obtain: You can view the API key for your account in the AddEvent dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: addevent-authentication
source_filename: addevent-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.addevent.com/reference/authentication.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.addevent.com/reference/authentication.md\nsources:\n- https://docs.addevent.com/reference/authentication.md\n- https://docs.addevent.com/reference/getting-started.md\ndescription: 'Authentication to the API is performed with HTTP Bearer Authentication. Provide your API key in the `Authorization` header when\n  making a request, as follows:'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authentication to the API is performed with HTTP Bearer Authentication. Provide your API key in the `Authorization` header when making\n    a request, as follows:'\n  location: header\n  header: Authorization\n  how_to_obtain: You can view the API key for your account in the AddEvent dashboard.\ndocs: https://docs.addevent.com/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/addevent/authentication/addevent-authentication.yml
summary_line: 1 scheme
tags:
- Calendar
- Integration
- Marketing
- API
- SaaS
- Events
---
