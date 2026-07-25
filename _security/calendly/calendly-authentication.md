---
api_key_in: []
api_specs:
- filename: calendly-webhook-api-asyncapi.yml
  format: yaml
  label: Calendly Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/asyncapi/calendly-webhook-api-asyncapi.yml
- filename: calendly-activity-log-api-openapi.yml
  format: yaml
  label: Calendly Activity Log API
  slug: calendly-activity-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-activity-log-api-openapi.yml
- filename: calendly-availability-api-openapi.yml
  format: yaml
  label: Calendly Availability API
  slug: calendly-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-availability-api-openapi.yml
- filename: calendly-data-compliance-api-openapi.yml
  format: yaml
  label: Calendly Data Compliance API
  slug: calendly-data-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-data-compliance-api-openapi.yml
- filename: calendly-event-types-api-openapi.yml
  format: yaml
  label: Calendly Event Types API
  slug: calendly-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-event-types-api-openapi.yml
- filename: calendly-groups-api-openapi.yml
  format: yaml
  label: Calendly Groups API
  slug: calendly-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-groups-api-openapi.yml
- filename: calendly-invitees-api-openapi.yml
  format: yaml
  label: Calendly Invitees API
  slug: calendly-invitees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-invitees-api-openapi.yml
- filename: calendly-organizations-api-openapi.yml
  format: yaml
  label: Calendly Organizations API
  slug: calendly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-organizations-api-openapi.yml
- filename: calendly-routing-forms-api-openapi.yml
  format: yaml
  label: Calendly Routing Forms API
  slug: calendly-routing-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-routing-forms-api-openapi.yml
- filename: calendly-scheduled-events-api-openapi.yml
  format: yaml
  label: Calendly Scheduled Events API
  slug: calendly-scheduled-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-scheduled-events-api-openapi.yml
- filename: calendly-shares-api-openapi.yml
  format: yaml
  label: Calendly Shares API
  slug: calendly-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-shares-api-openapi.yml
- filename: calendly-users-api-openapi.yml
  format: yaml
  label: Calendly Users API
  slug: calendly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-users-api-openapi.yml
- filename: calendly-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Calendly Webhook Subscriptions API
  slug: calendly-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-webhook-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/authentication/calendly-authentication.yml
summary_line: http · 1 scheme
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
---
