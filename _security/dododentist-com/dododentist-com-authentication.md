---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dododentist-com-appointments-api-openapi.yml
  format: yaml
  label: DodoDentist Appointments API
  slug: dododentist-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-appointments-api-openapi.yml
- filename: dododentist-com-clinics-api-openapi.yml
  format: yaml
  label: DodoDentist Clinics API
  slug: dododentist-com-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-clinics-api-openapi.yml
- filename: dododentist-com-invoices-api-openapi.yml
  format: yaml
  label: DodoDentist Invoices API
  slug: dododentist-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-invoices-api-openapi.yml
- filename: dododentist-com-patients-api-openapi.yml
  format: yaml
  label: DodoDentist Patients API
  slug: dododentist-com-patients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-patients-api-openapi.yml
- filename: dododentist-com-payments-api-openapi.yml
  format: yaml
  label: DodoDentist Payments API
  slug: dododentist-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-payments-api-openapi.yml
- filename: dododentist-com-treatments-api-openapi.yml
  format: yaml
  label: DodoDentist Treatments API
  slug: dododentist-com-treatments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-treatments-api-openapi.yml
- filename: dododentist-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: DodoDentist Webhook subscriptions API
  slug: dododentist-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dododentist Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DodoDentist secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DodoDentist
provider_slug: dododentist-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key secret>)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/dododentist-com-openapi.json
  type: http
- description: 'Operator session token issued by the DodoDentist dashboard: `Authorization: Token <access token>`.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/dododentist-com-openapi.json
  type: apiKey
slug: dododentist-com-authentication
source_filename: dododentist-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dododentist-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key\n    secret>)`.'\n  sources:\n  - openapi/dododentist-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the DodoDentist dashboard: `Authorization:\n    Token <access token>`.'\n  sources:\n  - openapi/dododentist-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dododentist-com/authentication/dododentist-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Dental
- Software
- Software-as-a-Service
- Practice Management
- Healthcare
---
