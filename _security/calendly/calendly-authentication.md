---
api_key_in: []
api_specs:
- filename: calendly-scheduling-api-openapi.yml
  format: yaml
  label: Calendly Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-scheduling-api-openapi.yml
- filename: calendly-webhook-api-asyncapi.yml
  format: yaml
  label: Calendly Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/asyncapi/calendly-webhook-api-asyncapi.yml
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
