---
api_key_in: []
api_specs:
- filename: savvycal-current-user-api-openapi.yml
  format: yaml
  label: SavvyCal Current User API
  slug: savvycal-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-current-user-api-openapi.yml
- filename: savvycal-events-api-openapi.yml
  format: yaml
  label: SavvyCal Events API
  slug: savvycal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-events-api-openapi.yml
- filename: savvycal-scheduling-links-api-openapi.yml
  format: yaml
  label: SavvyCal Scheduling Links API
  slug: savvycal-scheduling-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-scheduling-links-api-openapi.yml
- filename: savvycal-time-zones-api-openapi.yml
  format: yaml
  label: SavvyCal Time Zones API
  slug: savvycal-time-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-time-zones-api-openapi.yml
- filename: savvycal-webhooks-api-openapi.yml
  format: yaml
  label: SavvyCal Webhooks API
  slug: savvycal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-webhooks-api-openapi.yml
- filename: savvycal-workflows-api-openapi.yml
  format: yaml
  label: SavvyCal Workflows API
  slug: savvycal-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Savvycal Authentication
name_suffix: Authentication
oauth_flows: []
overview: SavvyCal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SavvyCal
provider_slug: savvycal
scheme_count: 1
schemes:
- description: 'Personal access tokens (prefixed with `pt_secret_`) or OAuth 2.0 access tokens. Include in the Authorization header as: `Authorization: Bearer <token>`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/savvycal-meetings-openapi.yml
  type: http
slug: savvycal-authentication
source_filename: savvycal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/savvycal-meetings-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access tokens (prefixed with `pt_secret_`) or OAuth 2.0 access tokens.\n    Include in the Authorization header as: `Authorization: Bearer <token>`'\n  sources:\n  - openapi/savvycal-meetings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/authentication/savvycal-authentication.yml
summary_line: http · 1 scheme
tags:
- Scheduling
- Calendar
- Appointments
- Availability
- Booking
- Meetings
- Webhook
---
