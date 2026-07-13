---
api_key_in: []
api_specs:
- filename: llms.txt
  format: yaml
  label: Acuity Scheduling API
  slug: acuity-scheduling-api
  spec_type: OpenAPI
  url: https://developers.acuityscheduling.com/llms.txt
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Acuity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Acuity Scheduling secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Acuity Scheduling
provider_slug: acuity
scheme_count: 2
schemes:
- description: HTTP Basic Auth using Acuity User ID and API Key
  name: basicAuth
  scheme: basic
  sources:
  - openapi/acuity-scheduling-api-openapi.yml
  type: http
- description: OAuth2 for multi-account integrations
  flows:
  - authorizationUrl: https://acuityscheduling.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://acuityscheduling.com/oauth2/token
  name: oauth2
  sources:
  - openapi/acuity-scheduling-api-openapi.yml
  type: oauth2
slug: acuity-authentication
source_filename: acuity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acuity-scheduling-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using Acuity User ID and API Key\n  sources:\n  - openapi/acuity-scheduling-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://acuityscheduling.com/oauth2/authorize\n    tokenUrl: https://acuityscheduling.com/oauth2/token\n    scopes: 1\n  description: OAuth2 for multi-account integrations\n  sources:\n  - openapi/acuity-scheduling-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuity/refs/heads/main/authentication/acuity-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Scheduling
- Appointments
- Calendar
- Booking
- HIPAA
- Webhooks
---
