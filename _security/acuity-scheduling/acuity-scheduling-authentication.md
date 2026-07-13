---
api_key_in: []
api_specs:
- filename: acuity-scheduling-asyncapi.yml
  format: yaml
  label: Acuity Scheduling Webhooks
  slug: webhooks-asyncapi
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuity-scheduling/refs/heads/main/openapi/acuity-scheduling-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acuity Scheduling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acuity Scheduling secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acuity Scheduling
provider_slug: acuity-scheduling
scheme_count: 1
schemes:
- description: HTTP Basic auth using your User ID as username and API Key as password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/acuity-scheduling-openapi.yml
  type: http
slug: acuity-scheduling-authentication
source_filename: acuity-scheduling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acuity-scheduling-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using your User ID as username and API Key as password\n  sources:\n  - openapi/acuity-scheduling-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuity-scheduling/refs/heads/main/authentication/acuity-scheduling-authentication.yml
summary_line: http · 1 scheme
tags:
- Appointment Scheduling
- Booking
- Calendar
- Scheduling
- Squarespace
---
