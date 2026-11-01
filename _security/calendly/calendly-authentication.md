---
anonymous_access: false
api_key_in: []
api_specs:
- filename: calendly-webhook-api-asyncapi.yml
  format: yaml
  label: Calendly Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/calendly/asyncapi/calendly-webhook-api-asyncapi.yml
- filename: calendly-availability-api-openapi.yml
  format: yaml
  label: Calendly Availability API
  slug: calendly-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-availability-api-openapi.yml
- filename: calendly-groups-api-openapi.yml
  format: yaml
  label: Calendly Groups API
  slug: calendly-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-groups-api-openapi.yml
- filename: calendly-organizations-api-openapi.yml
  format: yaml
  label: Calendly Organizations API
  slug: calendly-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-organizations-api-openapi.yml
- filename: calendly-shares-api-openapi.yml
  format: yaml
  label: Calendly Shares API
  slug: calendly-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-shares-api-openapi.yml
- filename: calendly-users-api-openapi.yml
  format: yaml
  label: Calendly Users API
  slug: calendly-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-users-api-openapi.yml
- filename: calendly-activitylog-api-openapi.yml
  format: yaml
  label: Calendly Activity Log API
  slug: calendly-activitylog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-activitylog-api-openapi.yml
- filename: calendly-contacts-api-openapi.yml
  format: yaml
  label: Calendly Contacts API
  slug: calendly-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-contacts-api-openapi.yml
- filename: calendly-datacompliance-api-openapi.yml
  format: yaml
  label: Calendly Data Compliance API
  slug: calendly-datacompliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-datacompliance-api-openapi.yml
- filename: calendly-eventtypes-api-openapi.yml
  format: yaml
  label: Calendly Event Types API
  slug: calendly-eventtypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-eventtypes-api-openapi.yml
- filename: calendly-locations-api-openapi.yml
  format: yaml
  label: Calendly Locations API
  slug: calendly-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-locations-api-openapi.yml
- filename: calendly-notetaker-api-openapi.yml
  format: yaml
  label: Calendly Notetaker API
  slug: calendly-notetaker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-notetaker-api-openapi.yml
- filename: calendly-outgoingcommunications-api-openapi.yml
  format: yaml
  label: Calendly Outgoing Communications API
  slug: calendly-outgoingcommunications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-outgoingcommunications-api-openapi.yml
- filename: calendly-routingforms-api-openapi.yml
  format: yaml
  label: Calendly Routing Forms API
  slug: calendly-routingforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-routingforms-api-openapi.yml
- filename: calendly-scheduledevents-api-openapi.yml
  format: yaml
  label: Calendly Scheduled Events API
  slug: calendly-scheduledevents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-scheduledevents-api-openapi.yml
- filename: calendly-webhooks-api-openapi.yml
  format: yaml
  label: Calendly Webhooks API
  slug: calendly-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-webhooks-api-openapi.yml
- filename: calendly-scheduling-links-api-openapi.yml
  format: yaml
  label: Calendly Scheduling Links API
  slug: calendly-scheduling-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendly/openapi/calendly-scheduling-links-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Calendly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calendly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calendly
provider_slug: calendly
scheme_count: 1
schemes:
- description: Personal access token or OAuth 2.1 access token. Include in the Authorization header as Bearer {token}.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/calendly-scheduling-api-openapi.yml
  type: http
slug: calendly-authentication
source_filename: calendly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/calendly-scheduling-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token or OAuth 2.1 access token. Include in the Authorization\n    header as Bearer {token}.\n  sources:\n  - openapi/calendly-scheduling-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/calendly/authentication/calendly-authentication.yml
summary_line: http · 1 scheme
tags:
- Appointments
- Automation
- Booking
- Calendar
- Meetings
- Scheduling
---
