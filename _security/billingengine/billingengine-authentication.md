---
anonymous_access: false
api_key_in: []
api_specs:
- filename: billingengine-customers-api-openapi.yml
  format: yaml
  label: BillingEngine Customers API
  slug: billingengine-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-customers-api-openapi.yml
- filename: billingengine-invoices-api-openapi.yml
  format: yaml
  label: BillingEngine Invoices API
  slug: billingengine-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-invoices-api-openapi.yml
- filename: billingengine-payments-api-openapi.yml
  format: yaml
  label: BillingEngine Payments API
  slug: billingengine-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-payments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Billingengine Authentication
name_suffix: Authentication
oauth_flows: []
overview: BillingEngine secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BillingEngine
provider_slug: billingengine
scheme_count: 1
schemes:
- description: 'The API key from the settings of your account, sent as "Authorization: Bearer <key>". Only available in the paid plans.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/billingengine-openapi.json
  type: http
slug: billingengine-authentication
source_filename: billingengine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/billingengine-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'The API key from the settings of your account, sent as \"Authorization: Bearer\n    <key>\". Only available in the paid plans.'\n  sources:\n  - openapi/billingengine-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/billingengine/authentication/billingengine-authentication.yml
summary_line: http · 1 scheme
tags:
- Invoicing
- Fintech
- Germany
- Small Business
---
