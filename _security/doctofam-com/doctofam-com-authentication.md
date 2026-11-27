---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: doctofam-com-appointments-api-openapi.yml
  format: yaml
  label: Doctofam Appointments API
  slug: doctofam-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-appointments-api-openapi.yml
- filename: doctofam-com-clinics-api-openapi.yml
  format: yaml
  label: Doctofam Clinics API
  slug: doctofam-com-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-clinics-api-openapi.yml
- filename: doctofam-com-invoices-api-openapi.yml
  format: yaml
  label: Doctofam Invoices API
  slug: doctofam-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-invoices-api-openapi.yml
- filename: doctofam-com-patients-api-openapi.yml
  format: yaml
  label: Doctofam Patients API
  slug: doctofam-com-patients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-patients-api-openapi.yml
- filename: doctofam-com-payments-api-openapi.yml
  format: yaml
  label: Doctofam Payments API
  slug: doctofam-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-payments-api-openapi.yml
- filename: doctofam-com-procedures-api-openapi.yml
  format: yaml
  label: Doctofam Procedures API
  slug: doctofam-com-procedures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-procedures-api-openapi.yml
- filename: doctofam-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Doctofam Webhook subscriptions API
  slug: doctofam-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Doctofam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doctofam secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Doctofam
provider_slug: doctofam-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key secret>)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/doctofam-com-openapi.json
  type: http
- description: 'Operator session token issued by the Doctofam dashboard: `Authorization: Token <access token>`.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/doctofam-com-openapi.json
  type: apiKey
slug: doctofam-com-authentication
source_filename: doctofam-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/doctofam-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key\n    secret>)`.'\n  sources:\n  - openapi/doctofam-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the Doctofam dashboard: `Authorization: Token\n    <access token>`.'\n  sources:\n  - openapi/doctofam-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/doctofam-com/authentication/doctofam-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Medical Practice Management
- Appointment Scheduling
- Billing and Insurance
---
