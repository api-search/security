---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-calendar-calendars-api-openapi.yml
  format: yaml
  label: Google Calendar Calendars API
  slug: google-calendar-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-calendars-api-openapi.yml
- filename: google-calendar-colors-api-openapi.yml
  format: yaml
  label: Google Calendar Colors API
  slug: google-calendar-colors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-colors-api-openapi.yml
- filename: google-calendar-acl-api-openapi.yml
  format: yaml
  label: Google Calendar Acl API
  slug: google-calendar-acl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-acl-api-openapi.yml
- filename: google-calendar-channels-api-openapi.yml
  format: yaml
  label: Google Calendar Channels API
  slug: google-calendar-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-channels-api-openapi.yml
- filename: google-calendar-events-api-openapi.yml
  format: yaml
  label: Google Calendar Events API
  slug: google-calendar-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-events-api-openapi.yml
- filename: google-calendar-settings-api-openapi.yml
  format: yaml
  label: Google Calendar Settings API
  slug: google-calendar-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-settings-api-openapi.yml
- filename: google-calendar-calendar-list-api-openapi.yml
  format: yaml
  label: Google Calendar Calendar Calendar List API
  slug: google-calendar-calendar-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-calendar-list-api-openapi.yml
- filename: google-calendar-freebusy-api-openapi.yml
  format: yaml
  label: Google Calendar Calendar Freebusy API
  slug: google-calendar-freebusy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-freebusy-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Calendar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Calendar secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Calendar
provider_slug: google-calendar
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-calendar-acl-api-openapi.yml
  - openapi/google-calendar-calendar-list-api-openapi.yml
  - openapi/google-calendar-channels-api-openapi.yml
  - openapi/google-calendar-events-api-openapi.yml
  - openapi/google-calendar-freebusy-api-openapi.yml
  - openapi/google-calendar-settings-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 18
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-calendar-acl-api-openapi.yml
  - openapi/google-calendar-calendar-list-api-openapi.yml
  - openapi/google-calendar-channels-api-openapi.yml
  - openapi/google-calendar-events-api-openapi.yml
  - openapi/google-calendar-freebusy-api-openapi.yml
  - openapi/google-calendar-settings-api-openapi.yml
  type: oauth2
slug: google-calendar-authentication
source_filename: google-calendar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-calendar-acl-api-openapi.yml, openapi/google-calendar-calendar-list-api-openapi.yml,\n  openapi/google-calendar-channels-api-openapi.yml, openapi/google-calendar-events-api-openapi.yml,\n  openapi/google-calendar-freebusy-api-openapi.yml, openapi/google-calendar-settings-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n \
  \ - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 18\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-calendar/authentication/google-calendar-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Availability
- Calendar
- Event
- Google
- Google Workspace
- Scheduling
---
