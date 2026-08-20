---
api_key_in:
- header
api_specs:
- filename: qminder-appointments-api-openapi.yml
  format: yaml
  label: Qminder Appointments API
  slug: qminder-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-appointments-api-openapi.yml
- filename: qminder-input-fields-api-openapi.yml
  format: yaml
  label: Qminder Input Fields API
  slug: qminder-input-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-input-fields-api-openapi.yml
- filename: qminder-lines-api-openapi.yml
  format: yaml
  label: Qminder Lines API
  slug: qminder-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-lines-api-openapi.yml
- filename: qminder-locations-api-openapi.yml
  format: yaml
  label: Qminder Locations API
  slug: qminder-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-locations-api-openapi.yml
- filename: qminder-tickets-api-openapi.yml
  format: yaml
  label: Qminder Tickets API
  slug: qminder-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-tickets-api-openapi.yml
- filename: qminder-users-api-openapi.yml
  format: yaml
  label: Qminder Users API
  slug: qminder-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-users-api-openapi.yml
- filename: qminder-webhooks-api-openapi.yml
  format: yaml
  label: Qminder Webhooks API
  slug: qminder-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qminder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qminder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qminder
provider_slug: qminder
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: X-Qminder-REST-API-Key
  sources:
  - openapi/qminder-openapi-original.json
  type: apiKey
slug: qminder-authentication
source_filename: qminder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qminder-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Qminder-REST-API-Key\n  sources:\n  - openapi/qminder-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/authentication/qminder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Queue Management
- Appointment Scheduling
- Visitor Management
- Customer Experience
- REST
- GraphQL
- Webhook
- Software-as-a-Service
---
